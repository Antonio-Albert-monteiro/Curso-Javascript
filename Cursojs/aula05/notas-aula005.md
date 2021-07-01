### métodos getElements

#### código fonte:
~~~ html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
				<meta charset="UTF-8">
				<title>Primeiros passos com DOM</title>
</head>
<body>
				<h1>Iniciando estudos com DOM</h1>
				<p>aqui vai os resultados</p>
				<p>aprendendo a usar o <strong>DOM</strong> em javascript</p>
				<div id="msg">Clique em mim</div>
				<div name="msg">gravida lectus ei</div>
				<div id="oi">snkksksksmsmmzmsmzg</div>
</body>
</html>
~~~
~~~ javascript
getElementsByTagName('h1')[0] // usado para pegar um item pela sua tag
getElementById() // usando para pegar um item pelo id
getElementsByName()[0] // usando para pegar o item pelo name
getElementsByClassName()[0] // usado para pegar o item pela class
~~~

#### Usando o getElementsByTagName():
~~~ javascript
var h1 = window.document.getElementsByTagName("h1")
window.document.write(h1.innerText)
~~~

#### Usando o getElementById()
~~~ javascript
var d = window.document.getElementById("msg")
d.innerText = "My name is Antonio"
~~~

#### Usando o getElementsByName()[0]
~~~ javascript
var d2 = window.document.getElementsByName("msg")[0]
d2.innerText = "Olá, mundo!"
~~~

#### Usando o getElementsByClassName()[0]
~~~ javascript
var c = windonw.document.getElementsByClassName("msg")
c.innerText = "Seja bem vinda"
~~~

#### Usando o querySelector()
~~~ javascript
var div4 = window.document.querySelector("div#oi")
d4.style.background = "green"
~~~


##### deixa eu dizer uma curiosidade:
~~~ javascript
h1.innerText // texto do h1 sem formatação
h1.innerHTML // texto do h1 com formatação ou seja ele pega as tag também
h1.style.color = "black" // assim alterar o estilo dele

("div#msg") // guando é id
("div.msg") // guando é class
~~~