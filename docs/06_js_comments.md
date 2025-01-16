# Comentarios en JavaScript

Los comentarios en JavaScript se pueden utilizar para explicar el código JavaScript y hacerlo más legible. 

Los comentarios en JavaScript también se pueden utilizar para evitar la ejecución al probar código alternativo.

## Comentarios en línea

Los comentarios de una sola línea comienzan con `//`.

JavaScript ignorará cualquier texto entre `//` y el final de la línea (no se ejecutará).

Este ejemplo utiliza un comentario de una sola línea antes de cada línea de código:

**Ejemplo:**
```js
// Cambia el encabezado:
document.getElementById("myH").innerHTML = "Mi primera página";

// Cambia el parrafo:
document.getElementById("myP").innerHTML = "Mi primer párrafo.";
```

En este ejemplo se utiliza un comentario de una sola línea al final de cada línea para explicar el código.

**Ejemplo:**
```js
let x = 5;      // Declara x, dale el valor 5
let y = x + 2;  // Declara y, dale el valor x + 2
```

## Comentarios en bloque

Los comentarios de varias líneas comienzan con `/*` y terminan con `*/`.

JavaScript ignorará cualquier código dentro de `/*` y `*/`.

Este ejemplo utiliza un comentario de varias líneas (un bloque de comentarios) para explicar el código.

**Ejemplo:**
```js
/*
El código a continuación cambiará
el encabezado con id="myH"
y el párrafo con id="myP"
en mi página web:
*/

document.getElementById("myH").innerHTML = "Mi primera página";
document.getElementById("myP").innerHTML = "Mi primer párrafo.";
```

> Lo más común que se utiliza son los comentarios de una sola línea. Los comentarios en bloque se utilizan a menudo para documentación formal.

## Comentarios para pruebas

El uso de comentarios para evitar la ejecución de código es adecuado para las pruebas de código.

Agregar `//` delante de una línea de código cambia las líneas de código de una línea ejecutable a un comentario.

Este ejemplo utiliza `//` para evitar la ejecución de una de las líneas de código.

**Ejemplo:**
```js
//document.getElementById("myH").innerHTML = "Mi primera página";
document.getElementById("myP").innerHTML = "Mi primer párrafo.";
```

Este ejemplo utiliza un bloque de comentarios para evitar la ejecución de varias líneas.

**Ejemplo:**
```js
/*
document.getElementById("myH").innerHTML = "Mi primera página";
document.getElementById("myP").innerHTML = "Mi primer párrafo.";
*/
```

## Conclusión

Los comentarios en JavaScript sirven para explicar y mejorar la legibilidad del código, además para desactivar partes del mismo durante pruebas. Existen comentarios de una sola línea, iniciados con `//`, y de varias líneas, delimitados por `/*` y `*/`. Los comentarios de una sola línea son más comunes, mientras que los de bloque se usan para documentación formal. Utilizar comentarios es útil para evitar la ejecución de código sin necesidad de eliminarlo por completo.
