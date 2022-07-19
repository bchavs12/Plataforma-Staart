# HTML

### Atributos

#### Define a linguagem do site

- lang="pt-br"

#### Define um caminho para um link

- href="...."

#### Define um caminho da imagem

- src="...."

#### Info do item ao passar o mouse

- title="Saiba mais"

#### Define um identificador exclusivo para o documento

- id="nome do id"

#### Define um identificador geral para melhor manipulação

- class="nome da class"

#### Define estilo de um elemento

- style="color:blue;"

#### Edita conteúdo dentro do HTML

- Contenteditable="true"

#### Arrasta itens

- draggable="true"

#### Desaparece o conteúdo

- hidden="true"

#### Define o modo de leitura

- dir="rtl"

#### Navegar através do conteúdo pelo tab

- tabindex="1"

#### Atribue video do youtube

- iframe

---

## Formulários

### inputs gerais

#### São utilizados em formulários

- Text (para textos normais)
- email (email@email.com.br)
- password (para senhas)
- submit (value="Enviar")
- button (value="Clicar")
- number (para apenas números)
- tel (55-01010-0101)

### inputs de duração

#### Usadas para controlar duração, tempo, hora, dia.

- date(01-01-2023)
- week(semana 22, 2023)
- month(19 de Agosto, 2023)
- time(11:33)
- datetime-local(01-01-2023 11:33)

## Inputs de mídia

#### São utilizados pora controlar mídias

- image (Anexar imagem)
- file (exportar algum arquivo)

## Inputs de opções

#### São utilizados para controlar uma escolha do usuário

- radio (elemento de ativar é desativar)
- checkbox (caixa de opções)
- range (Caixa de volume)

## Inputs avançados

#### Não muito utilizados, mas importantes conhece-los

- hidden( esconde elemento)
- url( colocar endereços )
- color (escolher uma cor pro seu formulário)
- search (Caixa de busca)
- reset (reseta o formulário)

### Atributos do form

#### for

- Utilizado no label para conectar com id do Input

#### value

- Dar uma descrição ao conteúdo

#### name

- igual o id

#### placeholder

- Acrescenta info no input para auxiliar

#### disable="true"

- desativa o campo do input

#### required="true"

- Para tornar um campo obrigatorio

### Tags form

#### textarea

- Definir uma area de texto
- atributo que define o tamanho rows="10" cols="10"

<select>
    <option>Item 01</option>
    <option>Item 02</option>
    <option>Item 03</option>
    <option>Item 04</option>
    <option>Item 05</option>
</select>

<textarea rows="10" cols="10"></textarea>

---

### Marcação de video

#### Atributos

#### Video do youtube

- Iframe

#### Video normal

- tag video
  - atributos: autoplay, muted controls, poster(coloca uma tumbnail até dar play no video)

---

# CSS

## Propriedades do CSS

### Posicinamento

#### Propriedade Position

- position: static, relative, absolute

#### Exemplos

header img {
position:absolute;
right: 10px;
}

### Alinhamento de texto

#### Propriedades de alinhamentos de texto

- text-align: center, right, left, justify, end;

### Propriedade Visibility

- A propriedade CSS de visibilidade pode mostrar ou ocultar um elemento sem afetar o layout de um documento. Ou seja. caso oculto, o elemento não aparecerá na página mas seu espaço continua sendo ocupado.

#### hidden

- desapareçe da tela mas ainda ocupa espaço.

#### Exemplo

header {
background-color: silver;
text-align: center;
visibility: hidden;
}

### backgrounds

#### Oque é a propridade background

- A propriedade CSS "background" é usada para definir os valores de fundo individuais em um único lugar na folha de estilo.

#### background-image

- Inserir uma imagem no css.

#### background-size

- define o tamanho da imagem inserida.

#### background-repeat

- Define se quer repetir ou não a imagem inserida.

#### background-position

- Define a posição da imagem inserida.

### Cores

#### hexaDecimais

- através de letras e números.

header{
background-color: #fffff
}

#### RGB

- Através de números.

header {
background-color: rgb(0 , 0, 0)
}

## Seletores

- É uma funcionalidade do CSS que permite selecionarmos qual elemento do HTML queremos customizar.

### Seletor de elementos

- seletor que usa elementos tags

h1{
font-size: 15px;
color: black;
}

### Seletor universal

- Todos os elementos da minha aplicação deve ter estas propriedades

\*{
font-size: 15px;
color: black;
}

## Classes

- Para Classse (.) para id (#)

- classes com nome ... serão estilizadas

#formacao {
color: blue;
}

## Pseudo-classes

### Oque são Pseudo-classes

- Uma pseudo-classe é uma palavra-chave adicionada a seltores que especifica um estado especial do elementos selecionado.
- Quando se quer adicionar uma customização para um botão somente quando o ponteiro do mouse passar por cima dele.

### para uso de acessibilidade

- Sempre que usar uso do hover, usar focus para uso de mouse e teclado dar o mesmo efeito.

a:hover, a:focus {background-color: silver;}

### Exemplos

a:link {background-color: yellow;}
a:focus {background-color: pink;}
a:hover {muda a cor ao passar o mouse}

## Pseudo-elementos

### antes e depois do conteúdo

a:before {
content:"Hello World "
}
a:after {
content: "Bye,Bye"
}

## Animações CSS
### Propriedades
- trasition
 - transition-duration
 - transition-delay
- 
## Animation
### Propriedades
- animation-name
- animation-duration
- animation-timing-fuction
- animation-delay
- aniamtion-iteration-count
- animation-direction
- animation-fill-mode
- animation-play-state

## Keyframes
### Propriedades
- from 
 - Para começar a animação em 0%.
- to
 - Para terminar a animação em 100%.
- Porcentagem
 - Uma porcentagem do tempo na sequência de animação em que o quadro-chave espeficado deve ocorrer.


## Especificação

- Todos os elementos "a" que tiverem o valor #formacao serão estilizados

a[href="#formacao"]{padding-left:50px;}

## Box Model

- Conceito de caixas.
- Tudo que esta no html e uma caixa
- e toda caixa tem seu tamanho
- Border, padding, marging em px

### O que é "px" no css?

- O "px" (ou pixel) é uma das várias medidas que podemos usar para definir altura, largura, tamanho de fonte, espessura de borda, margens preencimentos, etc. no HTML.

- Para utilizar essa unidade basta informar os CSS, o valor da medida que se deseja aplicar á um elemento e escrever "px" ao lado direito do valor:

h1 {
border: 1px solid black;
border-radius: 10px 20px 30px 40px;
box-shadow: -5px 5px 5px black;
margin: 10px 20px 30px 40px;
padding: 10px 20px 30px 40px;
}

## Responsividade
### Oque é a Responsividade
- É uma técnica para fazer com que um site adapte seu conteúdo para diferentes tamanhos de tela, seja notebooks, tablets, smartphones ou até mesmo smartwatches.

### Medidas responsivas
- rem, em , porcentagens

### Tipos de mídia
- Apartir de determinada resoluçãao mudar o comportamento da aplicação.

- @media screen and (max-width: 1024px) {
  p{color:red;
  }

- @media screen and (max-width: 840px) {
  p{color:pink;
  }
  - Até essa resolução ficara com essas porpriedades ao passar de 840px mudara o comportamento.

## Fontes no Css

### font-family

- Escolhe a forma das letras
- Medidas: arial, helvetica, sans-serif;

### font-size

- Tamanho das fontes
- Medidas: px, (em, rem):para responsividade

### font-style

- Estilo da fonte

### font-weight

- Deixar em negrito
- Medidas: bold, bolder, lighter, normal, 100 a 900

### line-height

- Tamanho da linha
- Medidas: px, em, rem, normal

### Fontes extermas (Google Fonts)

- É uma biblioteca com mais de 800 fontes livres licenciadas e um diretório web interativo para navegar na biblioteca.

#### Como Inserir

- No css colocar
- @import url(url da font pega no google Fonts)

## FlexBox
- 

## CSS-Grid
### Oque é o CSS-Grid
- É um sistema de estruturação de layout que o CSS fornece. Ele permite configurar layouts em duas dimensões (linhas e colunas). A junção de linhas e colunas formam uma grade o que dá o nome a esse sistema(grid).

### Propriedades
- Definir 
 - Display no container
 - As areas de templates(onde vai ser usado determinado conteúdo)
 - As colunas e linhas com (grid-template-columns)

### Medidas do CSS-Grid
- px, fr, colunas é linhas.

### Exemplos
main{
    display: grid;
    grid-template-areas:
    "um dois";
    grid-template-columns: auto 200px;
}

section{
    grid-area: um;
}

aside{
    grid-area: dois;
}
