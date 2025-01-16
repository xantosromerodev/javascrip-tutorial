# Output JavaScript

## Formas de visualización

JavaScript puede "mostrar" datos de diferentes maneras.

- Escribir en un elemento HTML, usando `innerHTML`.
- Escribir en un HTML output usando `document.write()`.
- Escribir en un cuadro de alerta, usando `window.alert()`.
- Escribiendo en la consola del navegador, usando `console.log()`.

## Usando `innerHTML`

Para acceder a un elemento HTML, JavaScript puede utilizar el método `document.getElementById(id)`.

El atributo `id` define el elemento HTML. La propiedad `innerHTML` define el contenido HTML.

**Ejemplo:**
```html
<!DOCTYPE html>
<html>
<body>

<h1>Mi primera pagina web</h1>
<p>Mi primer parrafo.</p>

<p id="demo"></p>

<script>
document.getElementById("demo").innerHTML = 5 + 6;
</script>

</body>
</html>
```

> Cambiar la propiedad `innerHTML` de un elemento HTML es una forma común de mostrar datos en HTML.

## Usando `document.write()`

Para fines de prueba, es conveniente utilizar `document.write()`.

**Ejemplo:**
```html
<!DOCTYPE html>
<html>
<body>

<h1>Mi primera pagina web</h1>
<p>Mi primer parrafo.</p>

<script>
document.write(5 + 6);
</script>

</body>
</html>
```

> El uso de `document.write()` después de cargar un documento HTML, **eliminará todo el HTML existente**.

**Ejemplo:**
```html
<!DOCTYPE html>
<html>
<body>

<h1>Mi primera pagina web</h1>
<p>Mi primer parrafo.</p>

<button type="button" onclick="document.write(5 + 6)">Probar</button>

</body>
</html>
```

> El método `document.write()` solo debe usarse para pruebas.

## Usando `window.alert()`

Puedes utilizar un cuadro de alerta para mostrar datos.

**Ejemplo:**
```html
<!DOCTYPE html>
<html>
<body>

<h1>Mi primera pagina web</h1>
<p>Mi primer parrafo.</p>

<script>
    window.alert(5 + 6);
</script>

</body>
</html>
```

Puedes omitir la palabra clave `window`.

En JavaScript, el objeto `window` es el objeto de alcance global. Esto significa que las variables, propiedades y métodos pertenecen por defecto al objeto `window`. Esto también significa que especificar la palabra clave `window` es opcional.

**Ejemplo:**
```html
<!DOCTYPE html>
<html>
<body>

<h1>Mi primera pagina web</h1>
<p>Mi primer parrafo.</p>

<script>
alert(5 + 6);
</script>

</body>
</html>
```

## Usando `console.log()`

Para fines de depuración, puedes llamar al método `console.log()` en el navegador para mostrar datos.

> Aprenderás más sobre depuración en un capítulo posterior.

**Ejemplo:**
```html
<!DOCTYPE html>
<html>
<body>

<script>
console.log(5 + 6);
</script>

</body>
</html>
```

## Imprimir en JavaScript

JavaScript no tiene ningún objeto de impresión ni métodos de impresión.

No puedes acceder a los dispositivos de salida desde JavaScript.

La única excepción es que puede llamar al método `window.print()` en el navegador para imprimir el contenido de la ventana actual.

**Ejemplo:**
```html
<!DOCTYPE html>
<html>
<body>

<button onclick="window.print()">Imprimir esta página.</button>

</body>
</html>
```
## Conclusión

En JavaScript, tenemos diversas formas de mostrar datos en una página web. Se pueden usar métodos como `innerHTML` para cambiar el contenido de un elemento HTML, `document.write()` para escribir directamente en el documento (aunque solo se recomienda para pruebas), `window.alert()` para mostrar datos en un cuadro de alerta, y `console.log()` para depuración en la consola del navegador. Recordar que JavaScript no tiene métodos de impresión, pero se puede usar `window.print()` para imprimir la página actual.
