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
# - Listas: Usadas Para Criar Listas No Documentos, Existem 2 Tipos são eles Ordernados e não Ordenadas
## Ordenada: com apartir do 1 em diante
```html
<ol>
<li>primeiro</li>
<li>Segundoo</li>
</ol>
```
## Não Ordenada: Não tem númeração
```html
<ul>
<li>Primeiro</li>
<li>Segundo</li>
<ul>
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


