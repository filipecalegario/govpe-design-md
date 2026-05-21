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

O Padrão Digital GOVPE é o design system que unifica e dá consistência aos
produtos digitais do Governo do Estado de Pernambuco. A própria documentação se
declara em desenvolvimento contínuo, sujeita a atualizações frequentes, e se
divide em guias para designers, para desenvolvedores e para o catálogo de
tokens. O sistema serve dois públicos: a cidadania, que usa portais e
formulários de serviço público, e as equipes internas das secretarias, que
operam sistemas de backoffice. Daí a personalidade institucional e sóbria, com
prioridade para clareza, legibilidade e acessibilidade.

A documentação trata acessibilidade como requisito, não como extra: cada
componente registra orientações de ARIA, navegação por teclado e foco visível.
Esse compromisso aparece já na GovBar, a barra superior obrigatória que
identifica a solução como parte do ecossistema do Estado, aponta para o portal
pe.gov.br e reúne ferramentas de acessibilidade (como ajuste de tamanho de fonte
e alternância de tema). A GovBar deve ser o primeiro elemento da página e o
primeiro na ordem de tabulação.

O sistema é distribuído como biblioteca React/Next.js em dois pacotes: 
`@uigovpe/components`, com os componentes, e `@uigovpe/styles`, com os tokens e
estilos. Um UI Kit no Figma compartilha a mesma nomenclatura de tokens, mantendo
design e código alinhados. A implementação se apoia no PrimeReact, retematizado
com as cores e formas do GOVPE; quando um componente herda nome do PrimeReact
(por exemplo Dropdown em vez de Select), a documentação preserva esse nome para
evitar ambiguidade. Componentes de sobreposição (Dialog, Menu, Tooltip) exigem
um UiProvider, e as molduras institucionais (GovBar, AdminSideBar, AdminUserBar)
exigem um LayoutProvider, que também governa o comportamento responsivo.

Os tokens são organizados em duas camadas. Há uma camada primitiva, com escalas
de cor por matiz (azul, vermelho, verde, amarelo e cinza), cada uma em cinco
intensidades (de `softest` a `strong`), e há uma camada semântica que dá papel
às cores. Este documento achata essas camadas em um único nível semântico,
porque essa é a forma de uso recomendada: prefira sempre o token de papel ao
valor primitivo. O Padrão GOVPE oferece tema claro e tema escuro; o claro é o
canônico e o descrito aqui. Como o formato alpha do DESIGN.md não modela
múltiplos temas, o tema escuro fica registrado apenas em prosa.

## Colors

A cor é descrita pela documentação em papéis empilhados, não em valores soltos.
Há uma camada de fundo (background), abaixo de tudo; sobre ela ficam as
superfícies (surface) que abrigam o conteúdo; e sobre as superfícies vêm o texto
e os contornos (outline). Cada papel tem seu próprio conjunto de tokens, e toda
a identidade gira em torno de um azul institucional profundo, contrastado com
neutros frios para que o azul permaneça como único acento de marca.

- **Primary (#0034b7):** azul institucional, a cor de ação por excelência. Cobre
  o botão principal de cada tela, links, seleção (checkbox, radio, switch), aba
  ativa, cabeçalho de tabela e foco. A versão `primary-strong` (#001a7a) atende
  estados de hover e pressionado e tinge a GovBar, e `primary-surface` (#e6f3ff)
  é o fundo tonal suave de realces, tags, mensagens informativas e painéis de
  menu.
- **Secondary (#494c57):** cinza-ardósia escuro, usado em texto secundário e em
  selos neutros, sem competir com o azul.
- **Neutral (#f8fafc):** quase branco frio. É o fundo geral das páginas e também
  o texto claro aplicado sobre superfícies escuras. As variações `neutral-soft`
  (#e7e9eb) e `neutral-medium` (#ced2d7) cobrem fundos discretos, divisores e
  contornos.
- **Surface (#ffffff):** branco puro que eleva cartões e campos acima do fundo,
  criando hierarquia por contraste de tom.
- **On-surface (#28272c):** quase preto, o texto padrão sobre superfícies claras,
  calibrado para leitura prolongada em portais de serviço.
- **Feedback:** quatro famílias semânticas comunicam estado. Sucesso usa verde
  (#2b6418), alerta usa amarelo (#ffb60c), erro e perigo usam vermelho
  (#ac1010), e informação reaproveita o azul primário. Cada família tem uma
  versão `strong` para hover e uma versão `surface` (clara) para o fundo de
  mensagens, toasts e tags, sempre com texto escuro para preservar o contraste.

Todos os pares de fundo e texto previstos para conteúdo respeitam o mínimo de
4.5:1 da WCAG AA. O único par intencionalmente abaixo desse limite é o estado
desabilitado, que por convenção (e por isenção da WCAG) sinaliza
indisponibilidade com baixo contraste.

## Typography

A tipografia usa uma única família, **Inter**, carregada via Google Fonts e
otimizada pelo `next/font`. Uma fonte só, em poucos pesos, reforça a sobriedade
institucional e simplifica o carregamento em conexões variadas. São três pesos:
regular (400) para texto corrido, medium (500) para rótulos de interface, e bold
(700) para títulos.

A escala de tamanhos vai de `caption` (0.75rem) a `display` (4rem), sobre uma
base de 1rem. A aplicação define a raiz em 14px, então os valores em rem rendem
um pouco menores na tela do que a referência usual de 16px; manter rem preserva
o comportamento responsivo do sistema.

- **Display e Headings (h1 a h4):** sempre em bold, com entrelinha apertada (1.2
  nos maiores, 1.4 nos menores) para dar presença a títulos sem desperdiçar
  espaço vertical.
- **Body (lg, md, sm):** em regular, com entrelinha de 1.5, calibrada para
  leitura confortável de textos longos.
- **Label:** em medium, para botões e rótulos de campo, onde o peso intermediário
  melhora a legibilidade em alvos pequenos.
- **Caption:** o menor tamanho, para apoio, metadados, legendas e selos
  compactos.

A biblioteca expõe um componente Typography que materializa essa escala: aceita
uma variante semântica (display, h1 a h6, p, span, label) e props de peso,
alinhamento e transformação de caixa, garantindo hierarquia textual consistente.

## Layout

O layout segue uma escala de espaçamento em múltiplos de 4px, com um meio-passo
de 2px para microajustes. Essa cadência regular cria ritmo visual consistente
entre formulários densos do backoffice e páginas mais arejadas de serviço ao
cidadão. Os passos nomeados (de `xxs` a `xxxl`) cobrem desde o preenchimento de
selos compactos até a separação entre grandes blocos de conteúdo.

A responsividade é centralizada no LayoutProvider, que define um breakpoint
global (padrão 1024px), persiste preferências no armazenamento local e seleciona
o template da aplicação (backoffice ou landing page). Pelo hook useLayout, os
componentes consultam esse breakpoint para alternar entre apresentações de
desktop e mobile, escondendo ou reorganizando elementos conforme a largura. Os
templates de referência mostram essa composição: o Backoffice combina a moldura
de navegação (AdminSideBar e AdminUserBar) com a área de conteúdo, e o Login usa
os componentes do design system junto a React Hook Form e Zod para formulários
validados.

## Elevation & Depth

A profundidade é discreta e serve à hierarquia, não à decoração. A primeira
estratégia é o contraste de tom: o fundo da página é o neutro frio (#f8fafc) e o
conteúdo principal repousa sobre superfícies brancas (#ffffff), o que separa as
camadas sem nenhuma sombra. Essa lógica de camadas (background abaixo, surface
acima) é a base da hierarquia visual do sistema.

A segunda estratégia, reservada a cartões que precisam flutuar, é uma sombra
suave e difusa, sem deslocamento, que envolve o elemento como um halo. São três
níveis: o baixo usa um cinza claro com desfoque amplo (20px), o médio um cinza
intermediário (15px) e o alto um cinza escuro mais concentrado (10px). No tema
escuro esses níveis convergem para um cinza único, já que o contraste de
luminância opera de forma diferente sobre fundos escuros.

## Shapes

O arredondamento é sutil e funcional. A escala `rounded` vai de 2px (`min`,
usado em caixas de seleção) a um valor efetivamente circular de 100px (`full`,
usado em selos, tags, chips, avatares e controles em formato de pílula). Os
controles de uso frequente, como botões e campos de entrada, adotam o raio médio
(8px), que suaviza o contorno o suficiente para parecer moderno sem perder a
formalidade institucional. Cartões e cabeçalhos de acordeão usam o raio grande
(16px) para destacar sua condição de contêiner, e radio buttons e avatares são
totalmente circulares.

A regra prática é manter coerência por família: elementos retangulares
interativos compartilham o raio médio, contêineres usam o raio grande, e apenas
selos, chips, avatares e tags adotam pílula ou círculo. Misturar cantos
arredondados e retos na mesma vista quebra a unidade visual.

## Components

Os componentes herdam os tokens semânticos por referência, de modo que uma
mudança em uma cor de papel se propaga a todos os elementos que a consomem. As
entradas registram apenas os tokens visuais essenciais; estados conduzidos
exclusivamente por contorno (foco, inválido) são descritos em prosa, já que o
formato não modela cor de borda. As orientações abaixo resumem o uso documentado
de cada família.

- **Botões:** representam a ação que o usuário pode executar. Há variantes por
  intenção (primário, secundário, perigo, sucesso, alerta, plain) e por estilo
  (preenchido, outline, link), além de três tamanhos. O primário deve ser único
  por tela, com label curta e orientada à ação; ícones entram apenas quando
  reforçam o significado. Hover apenas escurece o fundo, preservando o texto.
- **Campos de entrada:** texto, número, moeda, senha, máscara, área de texto,
  dropdown (seleção única, sempre com label), multiseleção (que mostra os itens
  escolhidos como pills), seletor de data (digitação ou calendário) e busca
  (idealmente com autocomplete e botão de limpar) compartilham a mesma anatomia:
  fundo branco, contorno neutro, texto escuro, raio médio e altura de 2.5rem.
  Todo campo deve estar vinculado a um label; o placeholder serve só como
  exemplo de formato, nunca como substituto do label, e o erro deve dar feedback
  imediato e legível por leitores de tela. O foco realça o contorno em azul com
  anel de foco; o inválido troca o contorno por vermelho; o desabilitado reduz a
  opacidade do conjunto.
- **Controles de seleção:** checkbox para múltiplas escolhas independentes (com
  estado indeterminado para seleção parcial), radio para escolha única e
  exclusiva, e switch para alternância binária com efeito imediato, sem botão de
  salvar. Quando ativos, todos preenchem com o azul primário (o switch usa a
  versão mais escura). As labels ficam à direita do controle.
- **Cartões:** contêineres que agrupam informações relacionadas em hierarquia de
  título, subtítulo e descrição, com no máximo duas ações visíveis e
  preenchimento generoso, opcionalmente elevados.
- **Tags, Badges e Chips:** todos em formato de pílula, mas com papéis distintos.
  A tag identifica, categoriza ou rotula (palavras curtas, nunca como botão de
  ação), em fundo suave de feedback com texto escuro. O badge é um indicador
  compacto de contagem (notificações, itens pendentes), em fundo sólido de
  feedback; sua versão pequena apenas sinaliza novidade, sem número. O chip
  representa um critério de filtro selecionado e removível pelo X, em azul
  primário sólido.
- **Avatar:** círculo de fundo neutro com a inicial gerada do nome ou um ícone em
  azul primário, para representar usuários.
- **Mensagens e Toasts:** comunicam o resultado de uma ação sem bloquear o fluxo,
  em fundo suave de feedback, texto escuro e contorno na cor plena da família. A
  Message permanece na interface (com ou sem título conforme a criticidade); o
  Toast é uma notificação breve, sobreposta a um canto e que some sozinha. Ambos
  compartilham a mesma aparência visual.
- **GovBar:** moldura institucional superior, obrigatória em todas as páginas, em
  azul escuro com texto claro, sempre fixa no topo e primeira na ordem de
  tabulação.
- **Sobreposições:** o painel de Menu usa o fundo azul claro (primary-surface)
  com itens em texto escuro. O Dialog é uma janela modal que interrompe o fluxo
  para uma decisão crítica, com cabeçalho e corpo sobre o neutro claro, ação
  primária em destaque e fechamento por botão secundário, ícone ou Esc; reduza
  cada diálogo a uma única decisão. Tooltips aparecem como etiquetas curtas no
  hover.
- **Navegação e dados:** abas (Tab) organizam conteúdos relacionados na mesma
  página, marcando a seleção com texto azul e traço inferior azul; use de 5 a 7
  abas e prefira o Stepper para tarefas sequenciais. O Stepper guia processos em
  etapas (até quatro), nas variações com ícones ou minimalista para mobile.
  Breadcrumbs apresentam a hierarquia como links azuis, com o item atual não
  clicável. O Accordion agrupa conteúdo expansível com cabeçalhos em negrito e
  raio grande. O Paginator divide grandes volumes em páginas, destacando a ativa
  e oferecendo Próxima e Anterior. A Table organiza dados em linhas e colunas
  (com ordenação e estilo listrado), cabeçalho em texto azul e células com
  divisórias horizontais sutis. O Divider é uma simples linha neutra de
  separação.
- **Backoffice:** a AdminSideBar é a navegação lateral (estados aberto e fechado,
  temas default e blue, em média de 5 a 7 links e até 9), com tooltip nos ícones
  quando recolhida; a AdminUserBar reúne a identificação do usuário, seu nível de
  acesso e o breadcrumb contextual.

## Do's and Don'ts

- Use o azul primário apenas para a ação mais importante de cada tela; múltiplos
  botões primários competem entre si e diluem a hierarquia.
- Prefira sempre referenciar o token semântico (por exemplo "primary" ou
  "danger") em vez de copiar o valor hexadecimal do primitivo.
- Inclua a GovBar em todas as páginas, fixa no topo e como primeiro elemento
  acessível por teclado, pois ela identifica a solução e oferece acessibilidade.
- Vincule todo campo de formulário a um label visível e use o placeholder apenas
  como exemplo de formato, dando feedback de erro imediato e legível.
- Mantenha o contraste mínimo de 4.5:1 entre texto e fundo para texto normal,
  reservando contrastes baixos exclusivamente para estados desabilitados.
- Posicione as labels de checkbox e radio à direita do controle e mantenha a
  ordem das opções previsível.
- Comunique feedback pela família semântica correta: verde para sucesso, vermelho
  para erro, amarelo para alerta e azul para informação.
- Garanta operação completa por teclado, foco visível e atributos ARIA
  correspondentes aos estados (expandido, selecionado, desabilitado, carregando).
- Não use mais de 7 abas, nem ultrapasse 4 etapas no Stepper, nem mais de 9 links
  na barra lateral; reorganize quando exceder esses limites.
- Não use tags no lugar de botões de ação, nem aninhe accordions dentro de
  accordions.
- Não misture cantos arredondados e retos na mesma vista; respeite o raio
  previsto para cada família.
- Não use mais de três pesos da Inter em uma mesma tela, nem substitua a família
  por outra fonte.
- Não esconda ações importantes em menus do tipo hambúrguer fora do contexto
  mobile, pois isso aumenta o tempo de tarefa.
- Não aplique as sombras de elevação como recurso decorativo; use-as apenas para
  sinalizar que um elemento flutua acima do conteúdo.
