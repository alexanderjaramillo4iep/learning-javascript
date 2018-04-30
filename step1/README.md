# Aprendiendo Javascript (paso 1)

Te invito a seguir el siguiente paso a paso
1. Crea una carpeta en la que vas a trabajar y a hacer los ejemplos
2. Crea dentro de la carpeta un archivo llamado `index.html`
3. Crea una estructura básica de html dentro de `index.html` (html, head, body)
4. Elementos del head
	1. Define un meta para que acepte tildes así `<meta charset="utf-8" />`
	2. Define un título para tu página con la etiqueta `<title>`
5. Elementos del body
	1. Define un título de nivel 2 `<h2>`
	2. Define un párrafo con `id="demo"` que contenga un texto de prueba (lo dejo a tu imaginación)
	3. Define un botón con atributo `onclick` así `<button type="button" onclick="">Haz click!</button>`

en el numeral 5.3 vemos que dejamos el `onclick` vacío, debido a que acá comenzaremos a probar el funcionamiento de javascript dandole **comportamiento** a nuestra página cuando este a éste botón le hagan click

vamos a agregar el siguiente comando dentro de las comillas del onclick
`document.getElementById("demo").innerHTML = "Modificado con JavaScript!"` que explicaré a continuación
* la primera palabra `document` es reservada de javascript y sirve para acceder a las propiedades y elementos de nuestro html
* la función (o método) `getElementById` nos permite realizar búsquedas en nuestro html sobre todos los elementos y obtener todos los que tengan el atributo id deseado.
	* En nuestro caso, queremos obtener el elemento con `id="demo"` que es un párrafo
* luego de tener el elemento deseado (el párrafo con id demo), por medio del atributo `innerHTML` podemos obtener o modificar el contenido de nuestro párrafo
	* Para el caso de obtenerlo basta con guardarlo en una variable así: `var contenidoP = document.getElementById("demo").innerHTML` para posteriormente trabajar con dicho contenido
	* Para el caso de modificarlo asignamos un nuevo valor al contenido así: `document.getElementById("demo").innerHTML = "Modificado con JavaScript!"` como es nuestro caso, lo cual hará que ahora nuestro párrafo, tenga el texto `Modificado con JavaScript!`

[continuar→](../../tree/step2)

[volver al inicio](../../)