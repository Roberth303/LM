# LM
## Estructura minima de una web
```html
<!DOCTYPE html>
<html>
<head>
	<title></title>
</head>
<body>

</body>
</html>
```
## 3 Formas de usar CSS en HTML
```html
1. Poniendo el CSS en la cabezera del HTML con el siguiente codigo:

	<style type="text/css">
		div {
            	background:#FFFFFF;
        	}
    	</style>

2. Poniendo directamente los atributos en las etiquetas como por ejemplo

	<p>¡Hola <span style="color:#FF0000">amigo lector</span>!</p>

3. Poniendo el CSS en un archivo externo, lo enlazamos al HTML con el siguiente código:

	<link rel="stylesheet" type="text/css" href="index.css" />
```
## Crear una lista sin ordenar con 5 ingredientes de una receta de cocina
```html
<!DOCTYPE html>
<html>
<head>
	<title>5 Ingredientes de Cocina</title>
	<meta charset="utf-8">
</head>
<body>
	<ul>
		<li>Huevos</li>
		<li>Leche</li>
		<li>Aceite</li>
		<li>Agua</li>
		<li>Sal</li>
	</ul>
</body>
</html>
```
## Como se puede incluir JavaScript en html
```html
Al igual que el CSS tenemos 3 formas de poner JavaScript en HTML

1. Lo metemos en el Head del HTML con las siguientes etiquetas:

	<script> "Aqui dentro va el código de JavaScript" </script>

2. Directamente en el Body:

	<body>
	<script>
		let d = new Date();
		document.body.innerHTML = "<h1>Time right now is:  " + d.getHours() + ":" + d.getMinutes() + ":" + d.getSeconds()
		"</h1>"
	</script>
	</body>

*Esto código JV nos da la hora.

3. Poner el JV en un archivo externo y enlazarlo al HTML:

	<script src="js/myscript.js"></script>
```
## Que diferencia hay entre una clase y una ID
```html
Una ID esta pensada para que el elemento que selecciones sea único, sin embargo las clases estan pensadas para definir el mismo estilo en varios elementos.
Por ejemplo no puedes asignarle un ID a varios elementos de la pagina, en cambio con una clase puedes asignar una misma clase a varios elementos.
```
## Codigo para que un enlace sea abierto en una página nueva
```html
	<a href="documento.html" target="_blank">Enlace</a>
```
## Que son las pseudoclases, y ejemplos
```html
	Las pseudoclases son palabras claves que se añaden a los selectores, con el se pueden cambiar las propiedades del estado especial del selector.
Ejemplos:
	p:hover {
		background-color: #F89B4D;
	}
*Cuando el ratón este encima del párrafo este cambiara de color.

	a:visited {
		color: blue;
	}
*Si en enlace ya ha sido visitado el color de este ahora sera azul.
```
## Explicación de los modelos de caja CSS (Margin, Border, Padding)
```html
La propiedad Margin(margen) Crea un espacio entre el objeto y los objetos que lo rodean, fuera del borde.

La propiedad Border permiten especificar el estilo, la anchura y el color del borde del elemento.

La propiedad Padding(Relleno) define un espaciado entre el borde y el contenido.
```
## Explica que son los selectores de CSS y pon ejemplos
```html
Los selectores definen sobre qué elementos se aplicará un conjunto de reglas.

* {
  margin: 0;
  padding: 0;
}
//se utiliza para seleccionar todos los elementos de la pagina.

p {
  ...
}
//Selecciona todas las etiquetas de tipo parrafo(<p>)
	
p span {
color: red; 
}
//Selecciona los span dentro de p
```
## Di a quien afectan los siguientes selectores
````html
p a { color: red; } //Afecta a todos los enlaces que hayan dentro de los parrafos\\
p > a { color: red; } //Afecta a tofos los enlaces que sean hijos directos de parrafos\\
h1 + h2 { color: red } //Afecta a los h2 adyacentes de h1\\
a[class] { color: blue; } //Afecta a todos los class\\
a[class="externo"] { color: blue; } //Afecta a todos los class que sean "externo"\\
a[href="http://www.ejemplo.com"] { color: blue; } //Afecta a todos los enlaces web que tengan dicha direccion\\
````
