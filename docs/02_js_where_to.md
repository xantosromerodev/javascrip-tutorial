# Where to JavaScript

## La etiqueta `<script>`

En HTML, el código JavaScript se inserta entre las etiquetas `<script>` y `</script>`.

**Ejemplo:**

```html
<script>
    document.getElementById("demo").innerHTML = "Mi primer programa JavaScript";
</script>
```

> Los ejemplos antiguos de JavaScript usaban un atributo `type`: `<script type="text/javascript">`. El atributo `type` no es obligatorio. JavaScript es el lenguaje de secuencias de comandos predeterminado en HTML.

## Funciones y eventos

Una función de JavaScript es un bloque de código que se puede ejecutar cuando se "invoca".

Por ejemplo, se puede llamar a una función cuando ocurre un evento, como cuando el usuario hace clic en un botón.

> Aprenderás mucho más sobre funciones y eventos en capítulos posteriores.

## JS en el `<head>` o `<body>` 

Puedes colocar cualquier cantidad de scripts en un documento HTML.

Los scripts se pueden colocar en la sección `<body>`, o en el `<head>` de una página HTML, o en ambas.

## JS en el `<head>`

En este ejemplo, se coloca una función de JavaScript en la sección `<head>` de una página HTML.

La función se invoca (llama) cuando se hace clic en un botón.

**Ejemplo:**

```html
<!DOCTYPE html>
<html>
<head>
<script>
function myFunction() {
  document.getElementById("demo").innerHTML = "Parrafo cambiado.";
}
</script>
</head>
<body>
<h2>JavaScript en el Head</h2>

<p id="demo">Un parrafo</p>
<button type="button" onclick="myFunction()">Ejecutar</button>

</body>
</html>
```

## JS en el `<body>`

En este ejemplo, se coloca una función de JavaScript en la sección `<body>` de una página HTML.

La función se invoca (llama) cuando se hace clic en un botón.

**Ejemplo:**

```html
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript en el Body</h2>

<p id="demo">Un parrafo</p>

<button type="button" onclick="myFunction()">Ejecutar</button>

<script>
function myFunction() {
  document.getElementById("demo").innerHTML = "Parrafo cambiado.";
}
</script>

</body>
</html>
```

> Colocar scripts en la parte inferior del elemento `<body>` mejora la velocidad de visualización, porque la interpretación de scripts ralentiza la visualización.

## JS externo

Los scripts también se pueden colocar en archivos externos.

**Ejemplo:**

Archivo externo: `script.js`

```html
function myFunction() {
  document.getElementById("demo").innerHTML = "Parrafo cambiado.";
}
```

Los scripts externos son prácticos cuando se utiliza el mismo código en muchas páginas web diferentes.

Los archivos JavaScript tienen la extensión de archivo `.js`

Para utilizar un script externo, coloque el nombre del archivo del script en el atributo `src` de una etiqueta `<script>`:

**Ejemplo:**

```html
<script src="script.js"></script>
```

Puedes colocar una referencia de script externa en `<head>` o `<body>` como desee.

El script se comportará como si estuviera ubicado exactamente donde se encuentra la etiqueta `<script>`.

> Los scripts externos no pueden contener etiquetas `<script>`.

## Ventajas de usar JS externo

Colocar scripts en archivos externos tiene algunas ventajas.

- Separa HTML y código.
- Hace que HTML y JavaScript sean más fáciles de leer y mantener.
- Los archivos JavaScript almacenados en caché pueden acelerar la carga de la página.

Para agregar varios archivos de script a una página, utilice varias etiquetas de `<script>`.

**Ejemplo:**
```html
<script src="myScript1.js"></script>
<script src="myScript2.js"></script>
```

## Referencias externas

Se puede hacer referencia a un script externo de 3 maneras diferentes.

- Con una URL completa (una dirección web completa)
- Con una ruta de archivo (como `/js/`)
- Sin ninguna ruta

Este ejemplo utiliza una URL completa para vincular a `myScript.js`.

**Ejemplo:**
```html
<script src="https://www.w3schools.com/js/myScript.js"></script>
```

Este ejemplo utiliza una ruta de archivo para vincular a `myScript.js`.

**Ejemplo:**
```html
<script src="/js/myScript.js"></script>
```

Este ejemplo no utiliza ninguna ruta para vincular a `myScript.js`.

**Ejemplo:**
```html
<script src="myScript.js"></script>
```

## Conclusión

JavaScript nos permite insertar código en HTML mediante las etiquetas `<script>`. Se puede colocar en las secciones `<head>` o `<body>` del documento, y en archivos externos con la extensión `.js`. Los scripts externos mejoran la organización y el mantenimiento del código. JavaScript también puede ejecutarse con eventos, como clics de botón, invocando funciones definidas. Colocar los scripts al final del `<body>` mejora la velocidad de carga.