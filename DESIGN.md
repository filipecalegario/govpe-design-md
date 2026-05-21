---
version: alpha
name: Padrão Digital GOVPE
description: Design system do Governo do Estado de Pernambuco para serviços digitais
colors:
  primary: "#0034b7"
  primary-strong: "#001a7a"
  primary-surface: "#e6f3ff"
  secondary: "#494c57"
  neutral: "#f8fafc"
  neutral-soft: "#e7e9eb"
  neutral-medium: "#ced2d7"
  surface: "#ffffff"
  on-surface: "#28272c"
  danger: "#ac1010"
  danger-strong: "#841d1d"
  danger-surface: "#ffe4e4"
  success: "#2b6418"
  success-strong: "#12400d"
  success-surface: "#eafbd7"
  warning: "#ffb60c"
  warning-strong: "#b77706"
  warning-surface: "#fff6ce"
typography:
  display:
    fontFamily: Inter
    fontSize: 4rem
    fontWeight: 700
    lineHeight: 1.2
  h1:
    fontFamily: Inter
    fontSize: 2.5rem
    fontWeight: 700
    lineHeight: 1.2
  h2:
    fontFamily: Inter
    fontSize: 2rem
    fontWeight: 700
    lineHeight: 1.2
  h3:
    fontFamily: Inter
    fontSize: 1.5rem
    fontWeight: 700
    lineHeight: 1.4
  h4:
    fontFamily: Inter
    fontSize: 1.25rem
    fontWeight: 700
    lineHeight: 1.4
  body-lg:
    fontFamily: Inter
    fontSize: 1.25rem
    fontWeight: 400
    lineHeight: 1.5
  body-md:
    fontFamily: Inter
    fontSize: 1rem
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: Inter
    fontSize: 0.875rem
    fontWeight: 400
    lineHeight: 1.5
  label:
    fontFamily: Inter
    fontSize: 0.875rem
    fontWeight: 500
    lineHeight: 1.4
  caption:
    fontFamily: Inter
    fontSize: 0.75rem
    fontWeight: 400
    lineHeight: 1.5
rounded:
  min: 2px
  xs: 4px
  sm: 6px
  md: 8px
  lg: 16px
  full: 100px
spacing:
  xxs: 2px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  xxl: 48px
  xxxl: 64px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.neutral}"
    rounded: "{rounded.md}"
    padding: 8px 16px
    height: 2.5rem
    typography: "{typography.label}"
  button-primary-hover:
    backgroundColor: "{colors.primary-strong}"
  button-secondary:
    backgroundColor: "{colors.neutral}"
    textColor: "{colors.primary}"
    rounded: "{rounded.md}"
    padding: 8px 16px
    typography: "{typography.label}"
  button-secondary-hover:
    backgroundColor: "{colors.primary-surface}"
  button-outline:
    textColor: "{colors.primary}"
    rounded: "{rounded.md}"
    padding: 8px 16px
    typography: "{typography.label}"
  button-link:
    textColor: "{colors.primary}"
    rounded: "{rounded.md}"
    padding: 8px 16px
    typography: "{typography.label}"
  button-danger:
    backgroundColor: "{colors.danger}"
    textColor: "{colors.neutral}"
    rounded: "{rounded.md}"
    padding: 8px 16px
    typography: "{typography.label}"
  button-danger-hover:
    backgroundColor: "{colors.danger-strong}"
  button-success:
    backgroundColor: "{colors.success}"
    textColor: "{colors.neutral}"
    rounded: "{rounded.md}"
    padding: 8px 16px
    typography: "{typography.label}"
  button-success-hover:
    backgroundColor: "{colors.success-strong}"
  button-warning:
    backgroundColor: "{colors.warning}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: 8px 16px
    typography: "{typography.label}"
  button-warning-hover:
    backgroundColor: "{colors.warning-strong}"
  button-plain:
    backgroundColor: "{colors.neutral-soft}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: 8px 16px
    typography: "{typography.label}"
  button-plain-hover:
    backgroundColor: "{colors.neutral-medium}"
  button-sm:
    rounded: "{rounded.md}"
    padding: 4px 16px
    height: 2rem
  button-lg:
    rounded: "{rounded.md}"
    padding: 12px 16px
    height: 3rem
  input-default:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: 8px 16px
    height: 2.5rem
    typography: "{typography.body-md}"
  input-disabled:
    backgroundColor: "{colors.neutral}"
    rounded: "{rounded.md}"
  dropdown:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: 8px 16px
    height: 2.5rem
    typography: "{typography.body-md}"
  textarea:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: 8px 16px
    typography: "{typography.body-md}"
  checkbox-checked:
    backgroundColor: "{colors.primary}"
    rounded: "{rounded.min}"
  radio-checked:
    backgroundColor: "{colors.primary}"
    rounded: "{rounded.full}"
  switch-checked:
    backgroundColor: "{colors.primary-strong}"
    rounded: "{rounded.full}"
  chip:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.neutral}"
    rounded: "{rounded.full}"
    padding: 4px 12px
    typography: "{typography.caption}"
  card:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.lg}"
    padding: "{spacing.lg}"
    typography: "{typography.body-md}"
  avatar:
    backgroundColor: "{colors.neutral}"
    textColor: "{colors.primary}"
    rounded: "{rounded.full}"
  tag-info:
    backgroundColor: "{colors.primary-surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.full}"
    padding: 4px 16px
    typography: "{typography.caption}"
  tag-secondary:
    backgroundColor: "{colors.neutral-soft}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.full}"
    padding: 4px 16px
    typography: "{typography.caption}"
  tag-success:
    backgroundColor: "{colors.success-surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.full}"
    padding: 4px 16px
    typography: "{typography.caption}"
  tag-warning:
    backgroundColor: "{colors.warning-surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.full}"
    padding: 4px 16px
    typography: "{typography.caption}"
  tag-danger:
    backgroundColor: "{colors.danger-surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.full}"
    padding: 4px 16px
    typography: "{typography.caption}"
  badge-info:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.neutral}"
    rounded: "{rounded.full}"
    padding: 4px 8px
  badge-secondary:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.neutral}"
    rounded: "{rounded.full}"
    padding: 4px 8px
  badge-success:
    backgroundColor: "{colors.success}"
    textColor: "{colors.neutral}"
    rounded: "{rounded.full}"
    padding: 4px 8px
  badge-warning:
    backgroundColor: "{colors.warning}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.full}"
    padding: 4px 8px
  badge-danger:
    backgroundColor: "{colors.danger}"
    textColor: "{colors.neutral}"
    rounded: "{rounded.full}"
    padding: 4px 8px
  message-info:
    backgroundColor: "{colors.primary-surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: "{spacing.md}"
    typography: "{typography.body-sm}"
  message-success:
    backgroundColor: "{colors.success-surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: "{spacing.md}"
    typography: "{typography.body-sm}"
  message-warning:
    backgroundColor: "{colors.warning-surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: "{spacing.md}"
    typography: "{typography.body-sm}"
  message-danger:
    backgroundColor: "{colors.danger-surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: "{spacing.md}"
    typography: "{typography.body-sm}"
  govbar:
    backgroundColor: "{colors.primary-strong}"
    textColor: "{colors.neutral}"
    padding: 0px 24px
    typography: "{typography.caption}"
  menu:
    backgroundColor: "{colors.primary-surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: 8px 0px
    typography: "{typography.body-sm}"
  dialog-header:
    backgroundColor: "{colors.neutral}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: "{spacing.md}"
    typography: "{typography.h4}"
  dialog-content:
    backgroundColor: "{colors.neutral}"
    textColor: "{colors.on-surface}"
    padding: "{spacing.md}"
    typography: "{typography.body-md}"
  accordion-header:
    textColor: "{colors.on-surface}"
    rounded: "{rounded.lg}"
    padding: 16px 18px
    typography: "{typography.label}"
  tab-active:
    textColor: "{colors.primary}"
    padding: 0px 16px
    typography: "{typography.label}"
  breadcrumb-link:
    textColor: "{colors.primary}"
    typography: "{typography.body-sm}"
  table-header:
    textColor: "{colors.primary}"
    padding: "{spacing.md}"
    typography: "{typography.label}"
  table-cell:
    textColor: "{colors.on-surface}"
    padding: "{spacing.md}"
    typography: "{typography.body-sm}"
---

# Padrão Digital GOVPE

## Overview

O Padrão Digital GOVPE é o design system que unifica a linguagem visual dos
serviços digitais do Governo do Estado de Pernambuco. Ainda em desenvolvimento
contínuo, ele busca garantir consistência entre os produtos das diversas
secretarias e atende dois públicos ao mesmo tempo: a cidadania, que acessa
portais e formulários de serviço público, e as equipes internas, que operam
painéis administrativos (backoffice). Por isso a personalidade do sistema é
institucional e sóbria, com forte ênfase em legibilidade e acessibilidade, em
vez de expressividade decorativa.

O sistema é distribuído como biblioteca React/Next.js em dois pacotes
complementares: `@uigovpe/components`, com os componentes, e `@uigovpe/styles`,
com os tokens e estilos. Há ainda um UI Kit no Figma que compartilha a mesma
nomenclatura de tokens, o que mantém design e código alinhados. A
implementação se apoia na biblioteca PrimeReact, retematizada com as cores e
formas do GOVPE. Componentes de sobreposição (diálogo, menu, tooltip) dependem
de um UiProvider, e os componentes de moldura institucional (GovBar, barra
lateral e barra de usuário do admin) dependem de um LayoutProvider, que também
expõe os breakpoints responsivos da aplicação.

Um traço marcante do sistema é a GovBar, a barra superior de identidade do
governo, em azul institucional escuro, que concentra acessos e ferramentas de
acessibilidade como ajuste de tamanho de fonte e alternância de tema. A partir
dela, o restante da interface se organiza em torno de um único azul de marca,
contrastado com neutros frios.

Os tokens são organizados em duas camadas. Há uma camada primitiva, com escalas
de cor por matiz (azul, vermelho, verde, amarelo e cinza), cada uma em cinco
intensidades (de `softest` a `strong`), e há uma camada semântica, que dá papel
às cores (texto, superfície, fundo, contorno e feedback). Este documento achata
essas duas camadas em um único nível semântico, porque é a forma de uso
recomendada: prefira sempre o token de papel ao valor primitivo.

O Padrão GOVPE oferece tema claro e tema escuro. O tema claro é o canônico e é o
descrito aqui. Como o formato alpha do DESIGN.md não modela múltiplos temas, o
tema escuro fica documentado apenas em prosa: ele inverte as intensidades das
escalas neutras e ajusta opacidades, preservando os mesmos papéis semânticos.

## Colors

A paleta gira em torno de um azul institucional profundo, que carrega a
identidade do Governo de Pernambuco e concentra toda a ação primária da
interface. Os neutros são frios (tendendo ao azul acinzentado), o que dá
sobriedade às superfícies e mantém o azul como único acento de marca. As cores
semânticas derivam de escalas primitivas de cinco intensidades, das quais o
sistema seleciona os papéis abaixo.

- **Primary (#0034b7):** azul institucional. É a cor de ação por excelência,
  reservada para o botão principal de cada tela, links, seleção (checkbox,
  radio, switch), abas ativas, cabeçalhos de tabela e foco. Sua versão
  `primary-strong` (#001a7a) cobre estados de hover e pressionado e tinge a
  GovBar, e `primary-surface` (#e6f3ff) é o fundo tonal suave para realces,
  tags, mensagens informativas e painéis de menu.
- **Secondary (#494c57):** cinza-ardósia escuro. Atua como cor de apoio em
  texto secundário e em selos neutros, sem competir com o azul.
- **Neutral (#f8fafc):** quase branco frio. É o fundo geral das páginas e
  também o texto claro aplicado sobre superfícies escuras (botões preenchidos,
  GovBar, badges sólidos). As variações `neutral-soft` (#e7e9eb) e
  `neutral-medium` (#ced2d7) cobrem fundos discretos, divisores e contornos.
- **Surface (#ffffff):** branco puro. Eleva cartões e campos de entrada acima
  do fundo da página, criando hierarquia por contraste de tom.
- **On-surface (#28272c):** quase preto. É o texto padrão sobre superfícies
  claras, escolhido para maximizar a leitura em portais de serviço.
- **Feedback:** quatro famílias semânticas comunicam estado. Sucesso usa verde
  (#2b6418), alerta usa amarelo (#ffb60c), erro e perigo usam vermelho
  (#ac1010), e informação reaproveita o próprio azul primário. Cada família tem
  uma versão `strong` para hover e uma versão `surface` (clara) para o fundo de
  mensagens, toasts e tags, sempre combinada com texto escuro para garantir
  contraste.

Todos os pares de fundo e texto previstos para conteúdo seguem o mínimo de
4.5:1 da WCAG AA. O único par intencionalmente abaixo desse limite é o estado
desabilitado, que por convenção (e por isenção da WCAG) sinaliza
indisponibilidade com baixo contraste.

## Typography

A tipografia usa uma única família, **Inter**, carregada via Google Fonts e
otimizada pelo `next/font`. Uma fonte só, em poucos pesos, reforça a sobriedade
institucional e simplifica o carregamento em conexões variadas. São usados três
pesos: regular (400) para texto corrido, medium (500) para rótulos de
interface, e bold (700) para títulos.

A escala de tamanhos vai de `caption` (0.75rem) a `display` (4rem), construída
sobre uma base de 1rem. Vale notar que a aplicação define a raiz em 14px, então
os valores em rem rendem um pouco menores na tela do que a referência padrão de
16px; manter rem preserva o comportamento responsivo do sistema.

- **Display e Headings (h1 a h4):** sempre em bold, com entrelinha apertada
  (1.2 nos maiores, 1.4 nos menores) para dar presença a títulos de página e de
  seção sem desperdiçar espaço vertical.
- **Body (lg, md, sm):** em regular, com entrelinha de 1.5, calibrada para
  leitura confortável de textos longos como instruções e termos de serviço.
- **Label:** em medium, para botões e rótulos de campo, onde um peso
  intermediário melhora a legibilidade em alvos pequenos.
- **Caption:** o menor tamanho, para textos de apoio, metadados, legendas e
  selos compactos.

O componente Typography da biblioteca materializa essa escala: ele aceita uma
variante semântica (display, h1 a h6, p, span, label) e props de peso,
alinhamento e transformação de caixa, garantindo que a hierarquia textual seja
aplicada de forma consistente.

## Layout

O layout segue uma escala de espaçamento baseada em múltiplos de 4px, com um
meio-passo de 2px para microajustes. Essa cadência regular cria ritmo visual
consistente entre formulários densos do backoffice e páginas mais arejadas de
serviço ao cidadão. Os passos nomeados (de `xxs` a `xxxl`) cobrem desde o
espaçamento interno de selos compactos até a separação entre grandes blocos de
conteúdo.

Componentes relacionados são agrupados em cartões com preenchimento interno
generoso, reforçando o princípio de contenção: itens que pertencem ao mesmo
contexto ficam visualmente reunidos sobre uma mesma superfície. A
responsividade é controlada pelo LayoutProvider, que expõe os breakpoints da
aplicação e permite que estruturas como a barra de usuário e a barra lateral do
admin alternem entre apresentações de desktop e mobile. Os templates de
referência (Backoffice e Login) demonstram a composição dessas molduras com a
área de conteúdo.

## Elevation & Depth

A profundidade é discreta e serve à hierarquia, não à decoração. Em vez de
sombras densas, o sistema usa duas estratégias combinadas. A primeira é o
contraste de tom: o fundo da página é o neutro frio (#f8fafc) e o conteúdo
principal repousa sobre superfícies brancas (#ffffff), o que separa as camadas
sem nenhuma sombra.

A segunda estratégia, reservada a cartões que precisam flutuar, é uma sombra
suave e difusa, sem deslocamento, que envolve o elemento como um halo. São três
níveis (baixo, médio e alto) que variam a intensidade do cinza e o raio de
desfoque: o nível baixo usa um cinza claro com desfoque amplo (20px), o médio um
cinza intermediário (15px) e o alto um cinza escuro mais concentrado (10px),
sempre sem deslocamento. No tema escuro, esses níveis convergem para um cinza
único, já que o contraste de luminância opera de forma diferente sobre fundos
escuros.

## Shapes

O arredondamento de cantos é sutil e funcional. A escala `rounded` vai de 2px
(`min`, usado em caixas de seleção) até um valor efetivamente circular de 100px
(`full`, usado em selos, tags, chips, avatares e controles em formato de
pílula). Os controles de uso frequente, como botões e campos de entrada, adotam
o raio médio (8px), que suaviza o contorno o suficiente para parecer moderno sem
perder a formalidade institucional. Cartões e cabeçalhos de acordeão usam um
raio maior (16px) para destacar sua condição de contêiner, e radio buttons e
avatares são totalmente circulares.

A regra prática é manter coerência por família: elementos retangulares
interativos compartilham o mesmo raio médio, contêineres usam o raio grande, e
apenas selos, chips, avatares e tags adotam o formato de pílula ou círculo.
Misturar cantos arredondados e retos na mesma vista quebra a unidade visual e
deve ser evitado.

## Components

Os componentes herdam os tokens semânticos por referência, de modo que uma
mudança em uma cor de papel se propaga para todos os elementos que a consomem.
As entradas de componente abaixo registram apenas os tokens visuais essenciais
(fundo, texto, tipografia, raio, preenchimento e dimensão); estados conduzidos
exclusivamente por contorno (foco, inválido) são descritos em prosa, já que o
formato não modela cor de borda.

- **Botões:** o sistema oferece variantes por intenção e por estilo. O primário
  (azul preenchido) é a ação principal e deve ser único por tela. O secundário
  (fundo claro, texto e contorno azuis) é a ação alternativa. As variantes
  outline e link removem o preenchimento e mantêm apenas o texto azul, para
  ações de menor peso. As variantes de feedback (perigo, sucesso, alerta)
  comunicam a consequência da ação, e a variante plain (cinza neutro) cobre
  ações terciárias. Há três tamanhos (pequeno, padrão e grande), que variam
  altura e preenchimento mantendo o mesmo corpo de texto. Todos compartilham o
  raio médio, e seus estados de hover apenas escurecem o fundo, preservando o
  texto.
- **Campos de entrada:** texto, área de texto, número, moeda, senha, máscara,
  dropdown, multiseleção, seletor de data e busca compartilham a mesma anatomia:
  fundo branco, contorno neutro, texto escuro, raio médio e altura de 2.5rem. O
  foco realça o contorno com o azul primário e um anel de foco azul claro; o
  estado inválido troca o contorno pelo vermelho de perigo; o estado
  desabilitado reduz a opacidade do conjunto em vez de recolorir o texto.
- **Controles de seleção:** checkbox, radio e switch, quando ativados, preenchem
  com o azul primário (o switch usa a versão mais escura). O checkbox usa o
  menor raio, o radio é circular e o switch tem formato de pílula.
- **Cartões:** superfície branca elevada, raio grande e preenchimento
  generoso, opcionalmente com um dos três níveis de elevação.
- **Tags, Badges e Chips:** todos em formato de pílula. As tags usam fundos
  suaves de feedback com texto escuro, para classificar conteúdo. Os badges
  usam fundos sólidos de feedback com texto claro (ou escuro, no caso do
  amarelo), para contagens e notificações de maior destaque. Os chips, em azul
  primário sólido, representam itens selecionáveis ou removíveis em campos de
  entrada.
- **Avatar:** círculo de fundo neutro com a inicial ou ícone em azul primário,
  usado para representar usuários.
- **Mensagens e Toasts:** comunicam estado em bloco, com fundo suave de
  feedback, texto escuro para máxima legibilidade e um contorno na cor plena da
  família correspondente. O Toast compartilha exatamente a aparência da Message,
  diferindo apenas por ser temporário e sobreposto.
- **GovBar:** barra institucional superior em azul escuro com texto claro,
  preenchimento horizontal e tipografia compacta; é a moldura de identidade do
  governo em todas as telas.
- **Menu e sobreposições:** o painel de menu usa o fundo azul claro
  (primary-surface) com itens em texto escuro e raio médio. Diálogos usam
  cabeçalho e corpo sobre o neutro claro, com o título em peso de subtítulo.
  Tooltips aparecem como pequenas etiquetas escuras com texto claro.
- **Navegação e dados:** abas marcam a seleção com texto azul e um traço
  inferior azul; breadcrumbs apresentam os níveis como links azuis; cabeçalhos
  de tabela usam texto azul em peso de rótulo, enquanto as células usam texto
  escuro com divisórias horizontais sutis; o acordeão usa cabeçalhos em negrito
  com raio grande. Paginadores destacam a página atual apenas pelo peso em
  negrito, e o divisor é uma simples linha neutra.

Componentes complexos (datepicker, stepper, paginador, multiseleção, tabela
completa) reutilizam esses mesmos tokens visuais; seu comportamento de
interação fica fora do escopo deste documento.

## Do's and Don'ts

- Use o azul primário apenas para a ação mais importante de cada tela; múltiplos
  botões primários competem entre si e diluem a hierarquia.
- Prefira sempre referenciar o token semântico (por exemplo, "primary" ou
  "danger") em vez de copiar o valor hexadecimal do primitivo.
- Mantenha o contraste mínimo de 4.5:1 entre texto e fundo para texto normal,
  reservando contrastes baixos exclusivamente para estados desabilitados.
- Escreva labels de botão curtas e orientadas à ação (por exemplo, "Enviar" ou
  "Baixar"), e use ícones apenas quando reforçarem o significado.
- Comunique feedback pela família semântica correta: verde para sucesso,
  vermelho para erro, amarelo para alerta e azul para informação.
- Garanta semântica e acessibilidade: botões com elemento nativo ou rótulo ARIA,
  estados desabilitado/ativo/carregando com atributos correspondentes, e
  operação completa por teclado.
- Não misture cantos arredondados e retos na mesma vista; respeite o raio
  previsto para cada família de componente.
- Não use mais de três pesos da Inter em uma mesma tela, nem substitua a família
  tipográfica por outra fonte.
- Não esconda ações importantes em menus do tipo hambúrguer fora do contexto
  mobile, pois isso aumenta o tempo de tarefa.
- Não aplique as sombras de elevação como recurso decorativo; use-as apenas para
  sinalizar que um elemento flutua acima do conteúdo.
