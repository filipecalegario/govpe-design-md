# Handoff: converter Padrão Digital GOVPE (Storybook) em DESIGN.md

## 1. Objetivo

Produzir um arquivo `DESIGN.md` no formato canônico do Google (spec em https://github.com/google-labs-code/design.md) que descreva o **Padrão Digital GOVPE**, design system do Governo de Pernambuco, hoje documentado em um Storybook publicado em:

```
https://ligadigital.pe.gov.br/storybook/index.html?path=/
```

O arquivo final precisa passar limpo no linter:

```
npx @google/design.md lint DESIGN.md
```

Idealmente sem erros, com warnings revisados caso a caso.

## 2. O que já foi tentado (e por que falhou)

Esta tentativa anterior rodou no claude.ai web, sem dev-browser:

1. `web_fetch` direto na URL do Storybook. Retornou apenas o shell HTML vazio porque o Storybook é uma SPA renderizada em JavaScript no cliente.
2. Tentativa de buscar `index.json` do Storybook. Bloqueada por restrição de permissão de URL não fornecida pelo usuário.
3. Busca por repositório público do GOVPE em GitHub e GitLab. Nada relevante encontrado (o que existe público é o gov.br federal, não o PE).
4. Conclusão: precisa de um navegador real que execute JS, daí o salto para o Claude Code com dev-browser.

## 3. Estratégia recomendada de extração

### 3.1. Primeiro, tente atalhos do Storybook (rápido)

Storybook expõe rotas internas que costumam estar acessíveis:

```
https://ligadigital.pe.gov.br/storybook/index.json
https://ligadigital.pe.gov.br/storybook/stories.json
https://ligadigital.pe.gov.br/storybook/project.json
```

Se algum deles responder, você terá o índice completo de stories (ids, títulos, paths) sem precisar varrer a sidebar visualmente. Use isso para montar a lista de páginas a visitar.

Para ver uma story isolada (sem o chrome do Storybook), use:

```
https://ligadigital.pe.gov.br/storybook/iframe.html?id=<story-id>&viewMode=story
```

E para a documentação MDX de cada componente:

```
https://ligadigital.pe.gov.br/storybook/iframe.html?id=<story-id>&viewMode=docs
```

### 3.2. Se nenhum atalho funcionar, vá pela UI

Abra a URL principal no dev-browser e navegue pela árvore lateral. Páginas a procurar (nomes variam):

- Introdução, Visão Geral, Brand, Identidade
- Cores, Color tokens, Paleta
- Tipografia, Typography, Fontes
- Espaçamento, Spacing, Grid
- Layout, Breakpoints, Containers
- Elevação, Sombras, Shadows
- Border radius, Shapes, Rounded, Cantos
- Iconografia (opcional, não vai pro DESIGN.md)
- Componentes (cada um com suas variantes: button, input, card, alert, modal, etc.)
- Acessibilidade, Diretrizes, Do's and Don'ts

### 3.3. Como extrair valores reais dos tokens

A doc pode mostrar amostras visuais sem expor o valor em texto. Quando isso acontecer:

1. Abra a story no `iframe.html?viewMode=story` para acessar o DOM real.
2. Use `getComputedStyle(elemento)` via console do dev-browser para ler cor, fonte, raio, padding, etc.
3. Procure por CSS custom properties no `:root` ou no documento: `getComputedStyle(document.documentElement)` lista todas as variáveis `--*`.
4. Inspecione o `<head>` por `<link rel="stylesheet">` apontando para um arquivo de tokens. Baixe e analise.

Storybook moderno também tem botão "Show code" no canvas que expõe o JSX e às vezes os props com valores.

## 4. Especificação do DESIGN.md (resumo operacional)

### 4.1. Estrutura do arquivo

```
---
# YAML front matter: tokens (machine-readable)
---

## Overview
## Colors
## Typography
## Layout
## Elevation & Depth
## Shapes
## Components
## Do's and Don'ts
```

Seções podem ser omitidas, mas as presentes devem aparecer **nessa ordem**. Cabeçalhos duplicados são erro de lint.

### 4.2. Schema dos tokens

```yaml
version: alpha
name: Padrão Digital GOVPE
description: Design system do Governo de Pernambuco
colors:
  primary: "#xxxxxx"
  secondary: "#xxxxxx"
  # ...
typography:
  h1:
    fontFamily: "..."
    fontSize: 3rem
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: "-0.02em"
  body-md:
    fontFamily: "..."
    fontSize: 1rem
rounded:
  sm: 4px
  md: 8px
  lg: 16px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.sm}"
    padding: 12px
  button-primary-hover:
    backgroundColor: "{colors.primary-container}"
```

### 4.3. Regras de tokens

- **Cores**: hex sRGB, com `#`, entre aspas.
- **Dimensões**: número + unidade (`px`, `em`, `rem`). Negativos permitidos em letter-spacing.
- **Referências**: `{path.to.token}` para apontar de um componente para um token global. Sempre prefira referenciar a duplicar valor.
- **Tipografia**: objeto com `fontFamily`, `fontSize`, `fontWeight`, `lineHeight`, `letterSpacing`, `fontFeature`, `fontVariation` (todos opcionais menos os usados).
- **Propriedades válidas em components**: `backgroundColor`, `textColor`, `typography`, `rounded`, `padding`, `size`, `height`, `width`. Mais nada (gera warning).
- **Variantes** (hover, active, pressed, focus, disabled): entrada separada com nome relacionado, ex.: `input-default`, `input-focus`, `input-disabled`.

### 4.4. Regras do linter (o que evitar)

- `broken-ref` (erro): referência `{x.y}` sem token correspondente.
- `missing-primary` (warning): definir cores sem ter um `primary`.
- `contrast-ratio` (warning): pares background/text abaixo de 4.5:1 (WCAG AA). Calcule antes.
- `orphaned-tokens` (warning): cor definida mas nunca usada por nenhum componente. Use ou remova.
- `missing-typography` (warning): cores sem nenhum token de tipografia.
- `section-order` (warning): seções fora da ordem canônica.

## 5. Pipeline sugerido

1. Acessar Storybook via dev-browser.
2. Tentar baixar `index.json`/`stories.json`. Se conseguir, montar lista de páginas a partir dele.
3. Visitar cada página de fundamento (cores, tipografia, espaçamento, etc.) e extrair tokens via DOM/computed styles/MDX.
4. Visitar cada componente, extrair propriedades de cada variante.
5. Construir o front matter YAML, preferindo referências `{colors.x}` em vez de valores duplicados.
6. Redigir a prosa de cada seção em português (ver seção 6 sobre estilo). Não copiar texto literal do site, **reescrever** para evitar problemas de copyright.
7. Salvar como `DESIGN.md`.
8. Rodar `npx @google/design.md lint DESIGN.md`. Resolver erros, revisar warnings.
9. Opcional: rodar `npx @google/design.md export --format css-tailwind DESIGN.md > theme.css` para gerar o tema Tailwind v4 de bônus.

## 6. Preferências de estilo (importante para a prosa)

O documento final será lido por humanos brasileiros, então:

- Português brasileiro com **acentos completos** em todas as palavras.
- **Nunca** usar travessões (em-dashes, `—`). Trocar por vírgulas ou parênteses.
- Aspas **antes** do ponto final, padrão brasileiro: `Ela falou "olá"`. e não `Ela falou "olá."`.
- Tom técnico, conciso, sem floreio. Cada seção da prosa deve explicar o **porquê** dos tokens, não repetir os valores.

## 7. Entregáveis esperados

1. `DESIGN.md` validado pelo linter do Google.
2. Lista das páginas/stories do Storybook efetivamente visitadas (rastreabilidade).
3. Log de findings do `lint` final, com justificativa para cada warning que não foi resolvido.
4. Opcional: `theme.css` exportado para Tailwind v4 e/ou `tokens.json` no formato DTCG.

## 8. Casos de borda a antecipar

- **Storybook sem documentação MDX**, só stories. Nesse caso, extração depende mais do DOM e computed styles.
- **Tokens semânticos vs primitivos**. Se o Padrão GOVPE tiver duas camadas (`color.brand.500` referenciada por `color.action.primary`), modelar a semântica nos componentes via referências `{}` e manter os primitivos como cores nomeadas no nível superior. O DESIGN.md não tem hierarquia profunda, então achata para um nível.
- **Fontes proprietárias**. Se houver fonte do governo (Rawline, por exemplo, comum em DS gov brasileiros), registrar o nome em `fontFamily` mesmo que o agente final precise carregar de outra forma.
- **Componentes muito complexos** (tabela, datepicker). Documentar só os tokens visuais essenciais; comportamento fica para a prosa.
- **Modo escuro**. Se o GOVPE tiver tema escuro, o DESIGN.md alpha não tem suporte multi-tema nativo. Mencionar na prosa de Overview e listar tokens do tema padrão (provavelmente o claro).

## 9. Referência rápida (exemplo mínimo válido)

```markdown
---
version: alpha
name: Padrão Digital GOVPE
description: Design system do Governo do Estado de Pernambuco
colors:
  primary: "#005AA7"
  on-primary: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#1A1A1A"
typography:
  h1:
    fontFamily: Rawline
    fontSize: 2.5rem
    fontWeight: 700
  body-md:
    fontFamily: Rawline
    fontSize: 1rem
    lineHeight: 1.5
rounded:
  sm: 4px
  md: 8px
spacing:
  sm: 8px
  md: 16px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.sm}"
    padding: 12px
---

## Overview

O Padrão Digital GOVPE estabelece a linguagem visual dos serviços
digitais do Governo de Pernambuco, priorizando acessibilidade,
sobriedade institucional e consistência entre secretarias.

## Colors

A paleta gira em torno do azul institucional GOVPE, contrastado com
neutros frios para garantir legibilidade em portais de serviço público.

(... e assim por diante ...)
```

Substituir os valores acima pelos reais coletados do Storybook.
