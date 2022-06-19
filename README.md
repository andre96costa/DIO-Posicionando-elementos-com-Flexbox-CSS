# Introdução ao flexbox 

## Flex Container
Tag que envolve os elementos, tag que recebe a prorpriedade flex, transforma todos os seus filhos em flex-items. Pode ser usado em qualquer tag.
- display: inicializa a propriedade flex.
- flex-direction: indica o posicionamento em que os flex-items estaram dispostos em coluna ou linha.
- flex-wrap: Quebra de linha
- flex-flow: Abreviação do flex-direction e flex-wrap, aplica os mesmos efeitos.
- justify-content: Alinha os itens dentro do container de acordo com uma direção.
- align-items: Alinha os items de acordo com o eixo x ou y.
- align-content: Alinha as linhas do container.

## Flex item
São os elementos filhos de um flex-container(dentro dele), podem se tornar flex-containers também.
- flex-grow: Fator de crescimento do item.
- flex-basis: Tamanho do item antes de ser aplicado a redistribuição de espaço.
- flex-shrink: Capacidade de redução do item.
- flex: Abreviação para flex-grow, flex-basis e flex-shrink, aplica as mesmas propriedades.
- order: Ordem de distribuição dos items dentro do container.
- align-self: Alinhamento de um item especifico.

## Propriedades
### display: flex
    Inicialisa a propriedade flex, cria um flex-container. Faz com que todos os flex-items fiquem disposição em linha, e os seus conteúdos fiquem adequados ao seu tamanho.
    Caso haja mais flex-items do que o flex-container suporta, os flex-items podem vazar.
### display-direction:
    É a propriedade que estabelece o eixo principal do container, definindo assim a direção que os flex-items são colocados no flex container. As propriedades reverse fazem com que os flex-items começem do lado direito da tela, também invertem a sequencia na qual os items começam.
    - row
    - row-reverse
    - column
    - column-reverse
### flex-wrap:
    É a propriedade que define se os itens devem ou não quebrar a linha. Por padrão eles não quebram linhas, isso faz com que os flex-itens sejam compactados além do limite do conteúdo e até o maximo do limite do flex-container.
    - nowrap:
    - wrap:
    - wrap-reverse:
### flex-flow:
    É um atalho para as propriedades flex-direction e flex-wrap. Porém seu uso não é tão comum, visto quem quando mudamos o flex-direction para column, mantemos o padrão do flex-wrap que é no-wrap.
    - row no-wrap
    - row wrap
    - row wrap-reverse
    - row-reverse no-wrap
    - row-reverse wrap
    - row-reverse wrap-reverse
    - column no-wrap
    - column wrap
    - column wrap-reverse
    - column-reverse no-wrap
    - column-reverse wrap
    - column-reverse wrap-reverse
### justify-content:
    Essa propriedade vai se encarregar de alinhar os itens dentro do container de acordo com a direção dos flex-item(flex-direction) e tratar da distribuição de espaçamento entre eles.
    Caso o flex-item esteja com alinhamento em linha, vai alinhas os item no eixo x, se estiver em coluna vai alinhas no eixo y.
    OBS: Caso os itens estejam ocupando 100% do espaço, a propriedade não se aplica.
    - center
    - flex-start
    - flex-end
    - space-between
    - space-around
### align-items
    Trata do alinhamento dos flex-itens de acordo com o eixo do container. O alinhamento é diferente para quando os itens estão em colunas ou linhas. Permite o alinhamento central no eixo vertical. Quando em linha, faz o alinhamento no eixo Y, quando em coluna faz o alinhamento no eixo X.
    - center
    - stretch
    - flex-start
    - flex-end
    - baseline
### flex-grow
    Define a proporcionalidade de crescimento dos itens, respeitando o tamanho de seus conteúdos internos. Respeitando o conteúdo interno.
    OBS: Não irá funcionar caso tenhamos adicionado justify-content ao flex-container.
### flex-basis
    É a propriedade que estabelece o tamanho inicial do item antes das distribuição de espaço restante dentro dele, usando como base o conteúdo interno disposto.