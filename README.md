# Caderno Virtual Sobre html <img src="https://cdn.icon-icons.com/icons2/2415/PNG/512/html_plain_wordmark_logo_icon_146476.png" height="50px" weight="50px" > e css <img src="https://cdn.icon-icons.com/icons2/2415/PNG/512/css_plain_wordmark_logo_icon_146574.png" height="50px" weight="50px" >
# <img src="https://cdn.icon-icons.com/icons2/2415/PNG/512/html_plain_wordmark_logo_icon_146476.png" height="50px" weight="50px" >HTML: A Base da Web
## (HyperText Markup Language, ou Linguagem de Marcação de Hipertexto em português) é a linguagem fundamental utilizada para criar a estrutura e o conteúdo das páginas da web.
# O que é tag ?
## As tags são códigos que usamos para construir uma página web. Elas são palavras-chave envoltas de menor que(<) e maior que(>) por Exemplo
```html
<p> <!--essa tag e para parágrafo-->
<h1> <!--essa tag e para Titulo-->
<img> <!--essa tag e para Imagem-->
```
## Essas tags contém o conteúdo visível da página.
# Atributos
## Os atributos são como pequenas notas que você adiciona a esses blocos para dar a eles instruções específicas. Eles modificam o comportamento ou a aparência de um elemento HTML
## Por que Usar Atributos?
## - Estilização: Definir classes para aplicar estilos CSS.
```html
<h1 class="titulo">Título da página</h1>
```
## - Indetificação: Para dar um Id único para o elemento para poder manipular com o JavaSript
```html
<p id="meu-paragrafo">Este é um parágrafo.</p>
```
## - Contéudo: para colocar links com o(href), ou imagens com (src) e formulários com o (value)
```html
<a href="https://www.google.com">Google</a> <!--Com Link-->
<img src="minha-imagem.jpg" alt="Descrição da imagem"> <!--Com Imagem-->
<input type="text" name="nome" value="Seu nome"> <!--Com Value-->
```
# Estruturas Básicas
## Uma página HTML básica possui a seguinte estrutura
```html
<!DOCTYPE html> 
<html>
<head>
<titile>Meu Primeiro Site</title>
</head>
<body>
<h1>Bem-vindo ao meu site!</h1>
<p>Este é um parágrafo de exemplo.</p>
</body>
<html>
```
## Explicação
## - <!DOCTYPEhtml>: Informa ao navegado que o um Documento HTML5
## - < html> < /html>: Define a raiz do documento html 
## - < head> < /head>: Define a cabeça do código onde o usuário não ver, podemos usar um link pra usar o css com html
## - < title> < /title>: Usamos essa tag dentro da tag head, ela define o Titulo que aparace na aba do navegador
## - < body< < /body>: Essa tag e o Corpo do Documento que é a parte visual do site onde podemos usar muitas tags
# Tags Básicas
# - Titulos: Vai do 1 até o 6, enquanto for menor número maior o titulo
```html
<h1>Maior</h1>
<h2>Maior</h2>
<h3>Maior</h3>
<h4>Maior</h4>
<h5>Maior</h5>
<h6>Maior</h6>
```
# - Parágrafos: Usada Para criar um Parágrafo no Documento
```html
<p>isso e um parágrafo</p>
```
# - Ânconra: Usada para criar hiperlinks, ou seja, elementos clicáveis que direcionam o usuário para outra página, um arquivo, um endereço de email, ou até mesmo para uma seção específica da mesma página.
```html
<a href="url_do_link">Texto do link</a>
```
# - Imagem: Usada Para Colocar uma Imagem no documento html.
```html
<img src="" alt="">
```
# - Botão: Usada Para Criar um botão No Documento
```html
<button>Clique Aqui</button>
```
# - Quebrar Linha: Usada Para Pular uma linha
```html
<br>
```
# <img src="https://cdn.icon-icons.com/icons2/2415/PNG/512/css_plain_wordmark_logo_icon_146574.png" height="50"  width="50"> CSS: A Linguagem que Define a Aparência das Páginas Web
## abreviação de Cascading Style Sheets (ou Folhas de Estilo em Cascata, em português), é uma linguagem de estilo usada para definir a apresentação visual de documentos HTML, como cores e tamanhos, o css e meio que uma maquiaguem para deixar mais bonita .
# Métodos de Usar o CSS no Html
## inline: E quando Usamos o css dentro da linha do código html
```html
<h1 style="color:red;">Hoje Foi legal</h1> <!--Aqui esse Titulo vai Sair Vermelho-->
```
## interno: E Quando colocamos na página do html o css, sendo que na cabeça onde o usuário não pode ver
```html
<!DOCTYPE html> 
<html>
<head>
<titile>Meu Primeiro Site</title>
<style>
h1{
color:red;
}
</style>
</head>
<body>
<h1>Bem-vindo ao meu site!</h1> <!--Aqui esse Titulo vai Sair Vermelho-->
<p>Este é um parágrafo de exemplo.</p>
</body>
<html>
```
## Externo: E Quando Criamos uma página só pro css e linkamos o css com o html
```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <title>css</title>
<link rel="stylesheet" href="style.css"> <!--Aqui estamos Juntando o css com o html-->

</head>

<body>
    <h1>Titulo da página</h1>
    <h2>Titulo da página</h2>
</body>
</html>
```
```css
h1 {
    color: blue;
    font-size: 15px;
}
```
# Organização Do CSS
## Podemos usar Várias maneiras, As Mais Utilizadas são por Id, class, nome
# ID: Só Pode ser utilizado Uma vez na página do Documento, Para indentidicar o id usamos#
```html
<h1 id="teste">Testando id</h1>
```
```css
#teste{
color:blue;
 font-size: 15px;
}
```
# Class: Diferente do id, na class podemos usar muitas vezes no codigo, Para indentificar usamos um ponto .
```html
<h1 class="hj">testando class</h1>
<p class="hj">Testando</p>
```
```css
.hj{
color:red;
font-size:12px;
}
```
# Cores: No CSS Existe 3 Tipos de Maneiras De Colocar as cores No Documento
## Nomes Das Cores: São Palavras chaves que representão palavras de cores comuns, São fáceis de lembrar e usar, mas oferecem um conjunto limitado de cores
```css
h1{
color:red; /* A cor do h1 vai ser vemelho*/
}
```
## Hexadecimal: Utiliza notação de seis Digitos Hexadecimais(#) epresentando a intensidade de vermelho, verde e azul (RGB)
```css
h1{
color: #FF0000;/* A cor do h1 vai ser vemelho*/
}
```
## RGB: Define a cor com base nas intensidades de vermelho, verde e azul, em valores de 0 a 255
```css
h1{
 rgb(255, 0, 0);/* A cor do h1 vai ser vemelho*/
}
```
# Bordas: são elementos visuais essenciais em CSS, permitindo que você adicione contornos e realce elementos em suas páginas web. Elas podem ser personalizadas em diversos aspectos, Os mais Utilizados são as Solid, Dotted, Dashed.
## Solid: é uma borda com uma linha normal
```css
  border:5px solid black; /*aqui essa borda vai ter 5 pixels, e a cor dela vai ser preta */
```
## dotted: Uma borda com linha pontilhada, com vários pontinhos
```css
  border:5px dotted black; /*aqui essa borda vai ter 5 pixels, e a cor dela vai ser preta */
```
## dashed: E Uma borda com linhas tracejadas
```css
  border:5px dashed black; /*aqui essa borda vai ter 5 pixels, e a cor dela vai ser preta */
```
## Arredondar Bordas : Para deixar uma borda meio que arredondado usamos o border-radius, permite que você crie cantos arredondados em elementos HTML, como divs, botões, imagens
```css
 border-radius: 200px;
````
## Posições: São fundamentais para definir as posições das bordas em um elemento CSS. Elas permitem um controle preciso sobre a aparência e o layout de seus elementos na página, existem 4 tipos são bottom,left,right,top
## Top: Acima do elemento a bordar vai ficar
```css
.meu-elemento {
  border-top: 2px solid black; /* Borda superior de 2px, sólida e preta */
}
```
## bottom: Abaixo do elemento a bordar vai ficar
```css
.meu-elemento {
  border-bottom: 2px solid black; /* Borda inferior de 2px, sólida e preta */
}
```
## left: A esquerda do elemento a bordar vai ficar
```css
.meu-elemento {
  border-left: 2px solid black; /* Borda esquerda de 2px, sólida e preta */
}
```
## right: A Direita do elemento a bordar vai ficar
```css
.meu-elemento {
  border-right: 2px solid black; /* Borda esquerda de 2px, sólida e preta */
}
```
# Padding: O espaço entre os elementos, o espaçamento interno
```css
padding:10px;
```
# Margin: O espaço extreno sobre o elemento, ou seja a área vazia sobre o elemento
```css
margin:12px;
```
# Altura e Largura: no html ou no css usamos os height e width, Podemos usar % para definir ou pixels/px
## Altura/height
```css
height:"12px";/*Usando pixels*/
height:"12%";/*Usando porcentagem*/
```
## Largura/width
```css
width:"12px";/*Usando pixels*/
width:"12%";/*Usando Porcentagem*/
```
# box-sizing: Existem dois tipos que são o content e border
## content-box: Digamos que você tem uma borda com as configurações de tamanho, e dentro dessa borda tem uma imagem, se você aumentar a imagem a borda não vai aumentar, só vai aumentar o contéudo que no caso vai ser a imagem
```css
box-sizing:content-box;
```
## border-box: Digamos que você tem uma borda, e dentro dela tem uma imagem, se você aumentar a imagem a bordar vai aumentar.
```css
box-sizing:border-box;
```
# Links: são elementos que conectam uma página da web a outra, seja dentro do mesmo site ou em um site diferente
## Tipos de Links
### - Links internos:Conectam a página dentro do mesmo site
### - Links extrenos: Conectam a páginas em outros sites
### - Links para arquivos: Conectam a arquivos como PDF, documentos do Word, etc
### - Links para âncoras: Conectam a partes específicas da mesma página.
## Atributos para a tag <a>
### - href: Indica para onde o link vai
### - target: Define onde o link será aberto, se colocarmos _blank, quando clicar vai abrir outra aba
### - title: Fornece um texto alternativo para o link, exibido ao passar o mouse.
### - rel: Especifica a relação entre a página atual e a página linkada.
# Formatação de texto em Html
## < b> < /b>:Deixa em Negrito
```html
<p>Testando <b>este</b></p>
```
## < strong> < /strong>:Deixa mais forte/negrito, Deixa com semântica de importância
```html
<p>teste <strong>forte</strong></p>
```
## < i> < /i>:Deixa o texto em italic
```html
<p>este e<i>Um texto em italic</i></p>
```
## < em> < /em>:Deixa em italic, mais com uma semântica de impotância
```html
<p>este e um<em>exemplo</em></p>
```
## < small> < /small>: Deixa o texto menor que o padrão
```html
<p>testando<small>menor</small></p>
```
## < del> < /del>:Deixa um risco no meio do texto
```html
<p>com<del>risco</del></p>
```
## < mark> </ mark>:Deixa o texto como se estivesse com um marca texto
```html
<p>com<mark>marca</mark</p>
```
## < sup> < /sup>: Deixa menor o texto e coloca sobe o texto
```html
<p>vai<sup>ser Menor</sup></p>
```
## < sub> < /sub>: Deixa Menor o texto e coloca abaixo do texto
```html
<p>abaixo<sub> do texto</sub></p>
```
# Formatação de texto no css
## E Quando você pode mudar a cor, tamanho, font, pode posicionar do texto com css
## Color: Pode mudar a cor do texto
```css
p{
color:red;/* a cor vai sair vermelho*/
}
```
## font-size: pode alterar o tamanho do texto
```css
.hs{
font-size:30px;
}
```
## font-weight: pode colocar em negrito
```css
.pj{
font-weight:bold;
}
```
## font-family: Pode alterar o modelo da fonte
```css
body{
  font-family: 'Lucida Sans';
}
```
## text-align: Pode posicionar o texto tem 4 tipos o right,left,center,justify
## - right: posiciona o texto para a Direita
```css
p{
text-align:right;
}
```
## - left: posiciona o texto para esquerda
```css
h1{
text-align:left;
}
```
## - center: posiciona no centro
```css
h1{
text-align:center;
}
```
## - Justify: deixa o texto justificado
```css
h1{
text-align:justify;
}
```
## text-decoration: Deixa o texto sem decoração, quando colocamos a tag <a> num texto ela fica com o anderlaine_, podemos tirar isso
```css
a{
text-decoration:none;
}
```
## text-transform: Pode Transformar o texto tem dois tipos o uppercase e o lowercase
## - uppercase: Deixa todo em Maiusculo/Caps Lock
```css
.kl{
text-transform:uppercase;
}
```
## - lowercase: Deixa todo em Minusculo
```css
.mn{
text-transform:lowercase;
}
```
## letter-space: Define o espaçamento entre cada letra do texto
```css
.hj{
letter-space:18px;
}
```
## word-space: Define o espaçamento entre cada palavra do texto
```css
.ls{
word-space:4px;
}
````
## line-height: Define o espaçamento entre as linhas
```css
p{
line-height:12px;
}
```
## text-shadow: Colocar um sombra no texto, tem 4 itens, e obrigatório colocar esse 4 itens, o Primeiro deles e a distância da sombra para a direita, o segundo e quão pra baixo vai a sombra, o terceiro e o espaço de espumaçado da sombra, o quarto e e a cor da sombra.
```css
p{
text-shadow: 2px 1px 2px red;
}
```
## Lista: Tem Dois Tipos de Listas ul,ol
## ul: Lista desordenada
```html
<ul>
<li>pri..</li>
<li>seg..</li>
</ul>
```
## Caso queira Mudar o Simbolo, teve usar o list-style-type, tem 4 Tipos o disc, square, cicle, none
## Disc: O padrão
```html
<ul style="list-style-type:disc;">
<li>Prim...</li>
<lisegu...</li>
</ul>
```
## Square: Um Quadrado
```html
<ul style="list-style-type:square;">
<li>Prim...</li>
<liSegu..</li>
</ul>
```
## Cicle: Um Circulo vazio por dentro
```html
<ul style="list-style-list:cicle;">
<li>Pri..</li>
<li>Seg..</li>
</ul>
```
## None: Nada só tem o espaçamento
```html
<ul style="list-style-list:none;"
<li>Prim..</li>
<li>Seg..</li>
</ul>
```
## ol: Lista Ordenada
```html
<ol>
<li>Prim..</li>
<li>Seg..</li>
</ol>
```
## Caso queria mudar, Colocamos o type, podemos mudar para o Alfabeto,Número,Algarimos Romano, Ou escolher em qual número começar
## Alfabeto
```html
<ol type="A">
<li>Prim...</li>
<li>Segu..</li>
</ol>
```
## Número/já está em número
```html
<ol type="1">
<li>Prim..</li>
<li>Seg..</li>
</ol>
```
## Algarismo Romano
```html
<ol type="I">
<li>Prim..</li>
<li>Seg..</li>
</ol>
```
## Caso queria escolher o número que vai começar, Usamos o start
```html
<ol start="12">
<li>Prim..</li>
<li>Seg</li>
</ol>
```




