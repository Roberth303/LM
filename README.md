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
