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
  input-default:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: 8px 16px
    typography: "{typography.body-md}"
  input-disabled:
    backgroundColor: "{colors.neutral}"
    rounded: "{rounded.md}"
  card:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.lg}"
    padding: "{spacing.lg}"
    typography: "{typography.body-md}"
  checkbox-checked:
    backgroundColor: "{colors.primary}"
    rounded: "{rounded.min}"
  tag-info:
    backgroundColor: "{colors.primary-surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.full}"
    padding: 4px 16px
  tag-secondary:
    backgroundColor: "{colors.neutral-soft}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.full}"
    padding: 4px 16px
  tag-success:
    backgroundColor: "{colors.success-surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.full}"
    padding: 4px 16px
  tag-warning:
    backgroundColor: "{colors.warning-surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.full}"
    padding: 4px 16px
  tag-danger:
    backgroundColor: "{colors.danger-surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.full}"
    padding: 4px 16px
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
  message-success:
    backgroundColor: "{colors.success-surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: "{spacing.md}"
  message-warning:
    backgroundColor: "{colors.warning-surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: "{spacing.md}"
  message-danger:
    backgroundColor: "{colors.danger-surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: "{spacing.md}"
---

# Padrão Digital GOVPE

## Overview

O Padrão Digital GOVPE é o design system que unifica a linguagem visual dos
serviços digitais do Governo do Estado de Pernambuco. Ele atende dois públicos
ao mesmo tempo: a cidadania, que acessa portais e formulários de serviço
público, e as equipes internas das secretarias, que operam painéis
administrativos (backoffice). Por isso a personalidade do sistema é
institucional e sóbria, com forte ênfase em legibilidade e acessibilidade, em
vez de expressividade decorativa.

O sistema é construído sobre a biblioteca de componentes PrimeReact, empacotada
no Next.js, e distribuído pelo pacote `@uigovpe/components`. As decisões de
estilo são materializadas em design tokens (variáveis CSS), o que mantém a
consistência entre telas públicas e telas administrativas e permite ajustes
centralizados.

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
sobriedade às superfícies e mantém o azul como único acento de marca.

- **Primary (#0034b7):** azul institucional. É a cor de ação por excelência,
  reservada para o botão principal de cada tela, links, seleção (checkbox,
  radio) e foco. Sua versão `primary-strong` (#001a7a) cobre os estados de
  hover e pressionado, e `primary-surface` (#e6f3ff) é o fundo tonal suave para
  realces, tags e mensagens informativas.
- **Secondary (#494c57):** cinza-ardósia escuro. Atua como cor de apoio em
  texto secundário e em selos neutros, sem competir com o azul.
- **Neutral (#f8fafc):** quase branco frio. É o fundo geral das páginas e
  também o texto claro aplicado sobre superfícies escuras (botões preenchidos).
  As variações `neutral-soft` (#e7e9eb) e `neutral-medium` (#ced2d7) cobrem
  fundos discretos, divisores e contornos.
- **Surface (#ffffff):** branco puro. Eleva cartões e campos de entrada acima
  do fundo da página, criando hierarquia por contraste de tom.
- **On-surface (#28272c):** quase preto. É o texto padrão sobre superfícies
  claras, escolhido para maximizar a leitura em portais de serviço.
- **Feedback:** quatro famílias semânticas comunicam estado. Sucesso usa verde
  (#2b6418), alerta usa amarelo (#ffb60c), erro e perigo usam vermelho
  (#ac1010), e informação reaproveita o próprio azul primário. Cada família tem
  uma versão `strong` para hover e uma versão `surface` (clara) para o fundo de
  mensagens e tags, sempre combinada com texto escuro para garantir contraste.

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
- **Caption:** o menor tamanho, para textos de apoio, metadados e legendas.

## Layout

O layout segue uma escala de espaçamento baseada em múltiplos de 4px, com um
meio-passo de 2px para microajustes. Essa cadência regular cria ritmo visual
consistente entre formulários densos do backoffice e páginas mais arejadas de
serviço ao cidadão.

Os passos nomeados (de `xxs` a `xxxl`) cobrem desde o espaçamento interno de
selos compactos até a separação entre grandes blocos de conteúdo. Componentes
relacionados são agrupados em cartões com preenchimento interno generoso,
reforçando o princípio de contenção: itens que pertencem ao mesmo contexto
ficam visualmente reunidos sobre uma mesma superfície.

A responsividade é controlada por um provedor de layout (LayoutProvider) que
expõe os breakpoints da aplicação, permitindo que componentes como a barra de
usuário administrativa alternem entre apresentações de desktop e mobile.

## Elevation & Depth

A profundidade é discreta e serve à hierarquia, não à decoração. Em vez de
sombras densas, o sistema usa duas estratégias combinadas. A primeira é o
contraste de tom: o fundo da página é o neutro frio (#f8fafc) e o conteúdo
principal repousa sobre superfícies brancas (#ffffff), o que separa as camadas
sem nenhuma sombra.

A segunda estratégia, reservada a cartões que precisam flutuar, é uma sombra
suave e difusa, sem deslocamento, que envolve o elemento como um halo. São três
níveis (baixo, médio e alto) que variam a intensidade do cinza e o raio de
desfoque: quanto mais alto o nível, mais escuro o cinza e mais concentrado o
desfoque. No tema escuro, esses níveis convergem para um cinza único, já que o
contraste de luminância opera de forma diferente sobre fundos escuros.

## Shapes

O arredondamento de cantos é sutil e funcional. A escala `rounded` vai de 2px
(`min`, usado em caixas de seleção) até um valor efetivamente circular de 100px
(`full`, usado em selos e tags em formato de pílula). Os controles de uso
frequente, como botões e campos de entrada, adotam o raio médio (8px), que
suaviza o contorno o suficiente para parecer moderno sem perder a formalidade
institucional. Cartões usam um raio maior (16px) para destacar sua condição de
contêiner.

A regra prática é manter coerência por família: elementos retangulares
interativos compartilham o mesmo raio médio, contêineres usam o raio grande, e
apenas selos e tags adotam o formato de pílula. Misturar cantos arredondados e
retos na mesma vista quebra a unidade visual e deve ser evitado.

## Components

Os componentes herdam os tokens semânticos por referência, de modo que uma
mudança em uma cor de papel se propaga para todos os elementos que a consomem.

- **Botões:** o sistema oferece variantes por intenção. O primário (azul
  preenchido) é a ação principal e deve ser único por tela. O secundário (fundo
  claro, texto azul) é a ação alternativa. As variantes de feedback (perigo,
  sucesso, alerta) comunicam a consequência da ação, e a variante plain (cinza
  neutro) cobre ações terciárias. Todos compartilham raio médio e preenchimento
  assimétrico (mais horizontal que vertical), e seus estados de hover apenas
  escurecem o fundo, preservando o texto.
- **Campos de entrada:** fundo branco, contorno neutro e texto escuro. O foco
  realça o contorno com o azul primário e um anel de foco azul claro; o estado
  inválido troca o contorno pelo vermelho de perigo; o estado desabilitado
  reduz a opacidade do conjunto em vez de recolorir o texto.
- **Cartões:** superfície branca elevada, raio grande e preenchimento
  generoso, opcionalmente com um dos três níveis de elevação.
- **Caixas de seleção:** quando marcadas, preenchem com o azul primário e usam
  o menor raio da escala, mantendo a marca de seleção em tom claro.
- **Tags e Badges:** ambos em formato de pílula. As tags usam fundos suaves de
  feedback com texto escuro, indicadas para classificar conteúdo. Os badges
  usam fundos sólidos de feedback com texto claro (ou escuro, no caso do
  amarelo), indicados para contagens e notificações de maior destaque.
- **Mensagens (inline):** comunicam estado em bloco, com fundo suave de
  feedback, texto escuro para máxima legibilidade e um contorno na cor plena da
  família correspondente.

Componentes complexos do sistema (tabela, datepicker, dropdown, paginador,
stepper, multiselect) reutilizam esses mesmos tokens visuais; seu comportamento
de interação fica fora do escopo deste documento.

## Do's and Don'ts

- Use o azul primário apenas para a ação mais importante de cada tela; múltiplos
  botões primários competem entre si e diluem a hierarquia.
- Prefira sempre referenciar o token semântico (por exemplo, "primary" ou
  "danger") em vez de copiar o valor hexadecimal do primitivo.
- Mantenha o contraste mínimo de 4.5:1 entre texto e fundo para texto normal,
  reservando contrastes baixos exclusivamente para estados desabilitados.
- Comunique feedback pela família semântica correta: verde para sucesso,
  vermelho para erro, amarelo para alerta e azul para informação.
- Não misture cantos arredondados e retos na mesma vista; respeite o raio
  previsto para cada família de componente.
- Não use mais de três pesos da Inter em uma mesma tela, nem substitua a família
  tipográfica por outra fonte.
- Não aplique as sombras de elevação como recurso decorativo; use-as apenas para
  sinalizar que um elemento flutua acima do conteúdo.
