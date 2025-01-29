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
# Tabelas: Usamos a tag table e dentro colocamos um tr e dentro um td e um th
## - < tr> </ tr>: Representa uma linha
## - < td> < /td>: Representa uma coluna
## - < th> < /th>: Representa o cabeçalho
```html
<table>
<tr>
<th>Comidas</th>
<th>Bebidas</th>
</tr>
<tr>
<td>Arroz</td>
<td>Café</td>
</tr>
<tr>
<td>Biscoito</td>
<td>Chá</td>
</tr>
<tr>
<td>Macarão</td>
<td>Suco</td>
</tr>
</table>
```
# hover: Quando Passamos o Mouse no elemento Pode Acontecer Algo
```css
a:hover{ 
color:red;/*a letra vai ficar vermelha*/
}
```
# Formulários: Usamos para o usuário preencher com informações, pode ser um texto ou email...
## < form> < /form>: tudo tem que estar dentro dessa tag
## < input>: aqui que vai ter os tipos.
## text: Da um campo de texto para o usuário digitar o que ele quiser.
```html
<form>
<input type="text">
</form>
```
## number: Da um campo de texto onde só pode digitar números
```html
<form>
<input type="number">
</form>
```
## password: Da um campo de texto onde pode digitar qualquer coisa, mas você não ver oque digitou fica com pontinhos, pos e uma senha
```html
<form>
<input type="password">
</form>
```
## checkbox: Um pequeno quadradro que podemos marcar apenas um ou mais, nele temos que colocar um name com o mesmo nome quem cada um se quiser poder marcar só um, se quiser marcar mais de 1 pode colocar name diferentes
```html
<form>
<input type="checkbox" name="frutas">
<input type="checkbox" name="frutas">
</form>
```
## radio: e a mesma coisa que o checkbox, só muda a forma que nesse e um circulo
```html
<form>
<input type="radio" name="Bebidas">
<input type="radio" name="Bebidas">
</form>
```
## submit: Um Botão Usado Para enviar o formulário
```html
<form>
<input type="number"> <!--o que for Digitado aqui-->
<input type="submit"> <!--Vai ser enviado ao clicar aqui-->
</form>
```
## email: Um campo de texto que só aceita email, ele percebe se tem o @
```html
<form>
<input type="email">
</form>
```
## date: Um caléndario que você pode escolher o dia mês e ano
```html
<form>
<input type="date">
</form>
```
## datetime-local: Um caléndario que pode colocar o tempo
```html
<form>
<input type="datetime-local">
</form>
```
## color: Pode colocar uma cor
```html
<form>
<input type="color">
</form>
```
## month: Um caléndario, agora só com o mês e ano
```html
<form>
<input type="month">
</form>
```
## range: um traço de tanto a tanto
```html
<form>
<input type="range">
</form>
```
## tel: um campo de texto para telefone
```html
<form>
<input type="tel">
</form>
```
## time: para a hora
```html
<form>
<input type="time">
</form>
```
## week: Pode colocar o caléndario, agora só vai a semana e ano
```html
<form>
<input type="week">
</form>
```
## select: apresenta um menu de opções onde, onde o usuário pode escolher as opções para essa tag funcionar dentro dela usamos a tag < option>
```html
<select>
<option>Abacaxi</option>
<option>Morango</option>
<option>Maçã</option>
</select>
```
## textarea: um campo de texto que pode aumentar o tamanho
```html
<form>
<input type="textarea">
</form>
```
## Button: faz a mesma coisa que o submit
```html
<form>
<input type="text">
<Button>Enviar<Button>
</form>
```
## Label: um texto para Especificar qual informação colocar no input, se no form colocarmos um id, e no label um for, conectando os, caso se eu clicar no label/texto, vai ativar
```html
<form>
<input type="text" id="aluno">
<label for="aluno">Digite aqui</label>
</form>
```
# legend, fieldset: Udados para Separar e organizar visualmente os inputs de um formulário por blocos.
## fieldset: Ele cria um campo ao redor do form.
```html
<form>
<fieldset>
<label>Nome Do aluno<br>
<input type="text" name="aluno">
</label>
</fieldset>
</form>
```
## legend: usada dentro do fieldset, coloca um texto no campo
```html
<form>
<fieldset>
<legend>Dados do aluno</legend>
<label>Nome Do aluno <br>
<input type="text" name="n-aluno">
</label><br>
<label>Idade do Aluno <br>
<input type="number" name="i-aluno">
</label>
</fieldset>
<fieldset>
<legend>Dados do Responsável</legend>
<label>Nome do Responsável <br>
<input type="text" name="r-respo">
</label><br>
<label> Idade do Responsável <br>
<input type="number" name="i-resp">
</label>
</fieldset>
</form>
```
# Validações nativas
## required: Se o campo de texto estiver vazio ele vai reconhecer
```html
<form>
<label>Digite seu nome: <br>
<input type="text" required>
</label>
</form>
```
## minlenght: o minimo de caracteres que pode colocar no campo de texto
```html
<form>
<labelDigite seu nome: <br>
<input type="text" minlenght="2"> <!--o Minino e 2, se tiver menos que 2 não vai-->
</label>
</form>
```
## maxlenght: o Máximo de caracteres que pode colocar no campo e texto
```html
<form>
<label Digite seu nome: <br>
<input type="text" maxlenght="10">  <!--o Máximo e 10, se tiver mais que 10 não vai-->
</label>
</form>
```
## step: no caso de inputs de number, com esse atributos podemos colocar com quantos números podemos pular
```html
<form>
<label>Digite seu idade: <br>
<input type="number" step="2">
</label>
</form>
```
## min: Define o minino de número dentro do campo
```html
<form>
<label>Digite qualquer número: <br>
<input type="number" min="1">
</label>
</form>
```
## max: Define o Máximo de número dentro do campo
```html
<form>
<label>Digite qualquer número: <br>
<input type="number" max="4">
</label>
</form>
```
## placeholder: E uma legenda que fica no campo de texto, meio que uma previa como vai ficar quando o campo for prenchido
```html
<form>
<label>Digite seu apelido:<br>
<input type="text" placeholder="dmd">
</label>
</form>
```
## Hidden: O input oculto é uma ferramenta útil para passar informações adicionais para o servidor de forma transparente para o usuário. Ao entender seu funcionamento e aplicações, você poderá criar formulários mais eficientes e seguros
```html
<form>
<input type="hidden" value="BR">
<label>Digite seu Nome: <br>
<input type="text" placeholder = "Lucas Vasconcelos">
</label>
</form>
```
## file: Pode puxar um arquivo do seu computador, tipo um pdf ou foto
```html
<form>
<input type="file">
</form>
```
# Unidades de Medidas Relativas (viewport)
## Ao invés de definir tamanhos em pixels ou outras unidades absolutas, as unidades relativas baseiam-se no tamanho da viewport do usuário (a área visível na tela, tem dois tipos que são o vh que são pra height, e vw para width,
### vh: viewport(height): Representa 1% da altura do viewport
```css
.informa{
background-color:red;
height:2vh;
}
```
### vw: viewport(width):Representa 1% da largura do wiewport
```css
.informa{
background-color:red;
width:5vw;
}
```
# header: é um cabeçalho que podemos colocar qualquer tag dentro dele
```html
<header>
<h1>Olá Mundo</h1>
</header>
```
# footer:um rotapê que pode colocar qualquer tag dentro dele
```html
<footer>
<h1>olá mundo</h1>
</footer>
```
# nav: usa para colocar link ou imagens, muito importante pós os monitores para deficientes, buscam essa tag
```html
<nav>
<a href=""></a>
<a href=""></a>
<img src="" alt="">
</nav>
```
# section: pode separar os assuntos do seu códigos em várias partes
```html
<section><!-- assunto 1 -->
<h1>Texto qualquer</h1>
<p>blablablabla</p>
</section>
```
# article: Usada para colocar o assunto Principal do site, o motor de busca vai procucar essa tag que deve estar com assunto principal
```html
<article>
<h1>Assunto Principal do meu site</h1>
</article>
```
# aside: Usada para o assunto secundário do site
```html
<article>
<h1>Assunto principal</h1>
<aside>
<h2>Assunto secundário</h2>
</aside>
</article>
```
# autofocus: Usada nos formulários, para quando aparecer já entrar pronto pra digitar 
```html
<form>
<input type="text" required placeholder="seu Nome.." autofocus >
</form>
```
# size: o campo com o tamanho que caiba n° caracteres, digamos se eu colocar size="20", vai ficar do tamanho que caiba 20 caracteres
```html
<form>
<label>Digite seu cpf
<input type="text" size="11">
</label>
```
# autocomplete: Digamos que você digitou algo no campo de texto antes, quando você for digitar novamente ai aparecer pra completar oque você digitou antes, tem como deixar ligado e desligado
```html
<input type="text" required placeholder="Digite seu nome aqui" autocomplete="off"> <!--Desligado-->
```
```html
<input type="text" required placeholder="Digite seu nome aqui" autocomplete="on"> <!--Ligado-->
```
# Degradê: permite criar transições suaves entre duas cores em elementos html
```css
background: linear-gradient(rgb(0, 0, 0),rgb(0, 0, 255));
```
# animação no css: economiza JavaScript usamos @keyframes para defenir temos duas maneiras os from{} to{}, e usando %
## usando to from
```css
@keyframes teste {
from{background-color:red;}
to{background-color:blue;}
}
.exemplo{
background-color:red;
width:100px;
height:100px;
animation-name:teste; /*ai vai o nome da animação, vai conectar*/
animation-duration: 5s; /*aqui vai a duração da animação, aqui no caso vai ficar 5 segundos*/
animation-iteration-count: infinite; /*aqui vai quantas vezes vai ser repetida, aqui no caso vai ser infinitamente*/
}
```
## usando %
```css
@keyframes testando{
    0%{
        background-color: red;
        border-radius: 12px;
        height: 100px;
    }
    25%{
        background-color: black;
        border-radius: 20px;
    }
    50%{
        background-color: aqua;
        border-radius: 30px;
    }
    75%{
        background-color: chartreuse;
        border-radius: 40px;
    }
    100%{
        background-color: pink;
        border-radius: 10px;
    }
}

.exemplo{
    background-color: red;
     height: 250px;
     width: 250px;
     animation-name: testando;
     animation-iteration-count: infinite;
     animation-duration: 5s;
}
```
# Sombra
## box-shadow: Colocar um sombra no background-color, tem 4 itens, e obrigatório colocar esse 4 itens, o Primeiro deles e a distância da sombra para a direita, o segundo e quão pra baixo vai a sombra, o terceiro e o espaço de espumaçado da sombra, o quarto e e a cor da sombra.
```css
.teste{
 width: 150px;
    height: 150px;
    background-color: green;
    box-shadow:#8888 5px 5px 0px;
}
```
# transições
## Permitem que você crie animações suaves e graduais entre dois estados de um elemento. Em vez de uma mudança de estilo acontecer instantaneamente, a transição cria um efeito visual mais agradável.
```css
.exemplo{
    background-color: red;
    width: 150px;
    height: 150px;
  margin: auto;
  margin-top: 5%;
  transition: all 2s linear; /*usamos a linear, vai durar 2 segundos*/
}
.exemplo:hover{ /* quando o curso do mouse estiver acima*/
    height: 100px;  /* vai ficar com 100px de altura*/
    width: 100px;  /* vai ficar com 100px de largura*/
    border-radius: 12px;  /* vai ficar com 12px de bordas*/
}
```
# Word-Wrap: é uma ferramenta essencial para controlar o layout de texto em CSS. Ao entender seus diferentes valores e como combiná-los com outras propriedades, você pode criar designs mais flexíveis e responsivos.
```css
p {
  width: 200px;
  word-wrap: break-word;
}
```
# lista de descrição
## uma lista de descrição, anteriormente conhecida como lista de definição, é uma estrutura semântica utilizada para relacionar termos com suas respectivas definições
## dl:Define a lista de descrição
```html
<dl></dl>
```
## dt:Define o termo da linha
```html
<dl>
<dt>
</dt>
</dl>
```
## dd:Define a descrição de um termo
```html
<dl>
<dt>
<dd></dd>
</dt>
</dl>
```
# citações//tem dois tipos
## 1-usadas em citações menores e coloca aspas
```html
<q></q>:
```
## 2-usadas em citações maiores coloca aspas
```html
<blockquote>
</blockquote>
```
# main: ela especifica o conteúdo principal da página, só pode ter uma por página
```html
<main>
<p>testando o main</p>
</main>
```
# address: usada para colocar informações de contatos e muito usada dentro da tag footer, dependendo do navegador a fonte vem em italic, mais pode mudar com o css se não quiser em italic
```html
<address>
</address>
```
# figure: Usada para juntar uma imagem com uma legenda, dentro dessa tag colocamos outra tag chamada figcaption que vem a legenda
```html
<figure>
<img src="https://www.google.com.br/google.jpg"/>
<figcaption>Logo do Google</figcaption> <!-- aqui vem a legenda-->
</figure>
```
# Flexbox: Layout que permite que os elementos responsivos, dentro de um contêiner, sejam organizados automaticamente
# Flex container
## - display: tem dois tipos que são o flex e o block
## -flex: deixa um elemento ao lado do outro
```html
<minha class="testando"> <!-- ops eu posso criar uma tag com qualquer nome, menos com nome de tags que já existem-->
<div>1</div>
<div>2</div>
<div>3</div>
</minha>
<style>
.testando{
display:flex; /*por padrão seria um elemento ao lado do outro. colocando isso vai fica um ao lado do outro */
}
div{
margin: 1%;
height:100px;
width:100px;
background-color: green;
}
</style>
```
## - block: deixa abaixo do outro, como no padrão
```html
<minha class="testando"> <!-- ops eu posso criar uma tag com qualquer nome, menos com nome de tags que já existem-->
<div>1</div>
<div>2</div>
<div>3</div>
</minha>
<style>
.testando{
display:block;
}
div{
margin: 1%;
height:100px;
width:100px;
background-color: green;
}
</style>
```
## flex-direction: Define a direção dos flex itens. Por padrão ele é row (linha), por isso (quando o display: flex; é adicionado), os elementos ficam em linha, um do lado do outro, tem 4 tipos que são row, row-reverse, column, column-reserve.
## row: em forma de linha horizontalmente, um ao lado do outro
```html
<minha class="testando"> <!-- ops eu posso criar uma tag com qualquer nome, menos com nome de tags que já existem-->
    <div>1</div>
    <div>2</div>
    <div>3</div>
    </minha>
    <style>
    .testando{
    display:flex;
    flex-direction:row;
    }
    div{
    margin: 1%;
    height:100px;
    width:100px;
    background-color: green;
    }
  </style>
```
## row-reverse: em forma de linha horizontalmente, da direita para esquerda
```html
<minha class="testando"> <!-- ops eu posso criar uma tag com qualquer nome, menos com nome de tags que já existem-->
    <div>1</div>
    <div>2</div>
    <div>3</div>
    </minha>
    <style>
    .testando{
    display:flex;
    flex-direction:row-reverse;
    }
    div{
    margin: 1%;
    height:100px;
    width:100px;
    background-color: green;
    }
  </style>
```
## column: em forma de coluna, um a baixo do outro, como no padrão
```html
<minha class="testando"> <!-- ops eu posso criar uma tag com qualquer nome, menos com nome de tags que já existem-->
  <div>1</div>
  <div>2</div>
  <div>3</div>
  </minha>
  <style>
  .testando{
  display:flex;
  flex-direction:column;
  }
  div{
  margin: 1%;
  height:100px;
  width:100px;
  background-color: green;
  }
</style>
```
## column-reverse: em forma de coluna, de baixo pra cima
```html
<minha class="testando"> <!-- ops eu posso criar uma tag com qualquer nome, menos com nome de tags que já existem-->
  <div>1</div>
  <div>2</div>
  <div>3</div>
  </minha>
  <style>
  .testando{
  display:flex;
  flex-direction:column-reverse;
  }
  div{
  margin: 1%;
  height:100px;
  width:100px;
  background-color: green;
  }
</style>
```
## flex-wrap: define se os itens podem quebrar linhas ou não temos 3 opções wrap,nowrap,wrap-reverse
## wrap: se o elemento não der vai quebrar a linha.
```html
<style>
      .container{
        background-color: #cccc;
        display: flex;
        flex-wrap: wrap;
    }
    .container div{
        background-color: red;
        margin:10px;
        padding: 10px;
        font-size: 18px;
    width: 200px;
    
    }
</style>
<body>
<div class="container">
 <div>1</div>
 <div>2</div>
 <div>3</div>
 <div>4</div>
 <div>5</div>
 <div>6</div>
 <div>7</div>
 <div>8</div>
 <div>9</div>
 <div>10</div>
</div>
```
## nowrap: não permite a quebra de linha.
```html
<style>
      .container{
        background-color: #cccc;
        display: flex;
        flex-wrap: nowrap;
    }
    .container div{
        background-color: red;
        margin:10px;
        padding: 10px;
        font-size: 18px;
    width: 200px;
    
    }
</style>
<body>
<div class="container">
 <div>1</div>
 <div>2</div>
 <div>3</div>
 <div>4</div>
 <div>5</div>
 <div>6</div>
 <div>7</div>
 <div>8</div>
 <div>9</div>
 <div>10</div>
</div>
```
## wrap-reverse: Quebra a linha assim que um dos flex itens não puder mais ser compactado. A quebra é na direção contrária, ou seja para a linha acima
```html
<style>
      .container{
        background-color: #cccc;
        display: flex;
        flex-wrap: wrap-reverse;
    }
    .container div{
        background-color: red;
        margin:10px;
        padding: 10px;
        font-size: 18px;
    width: 200px;
    
    }
</style>
<body>
<div class="container">
 <div>1</div>
 <div>2</div>
 <div>3</div>
 <div>4</div>
 <div>5</div>
 <div>6</div>
 <div>7</div>
 <div>8</div>
 <div>9</div>
 <div>10</div>
</div>
```























