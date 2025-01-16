# Introduccion a JavaScript

Este tutorial contiene algunos ejemplos de lo que JavaScript puede hacer.

## JS puede cambiar el contenido

Uno de los tantos métodos de HTML para JavaScript es `getElementById()`.

El siguiente ejemplo "encuentra" un elemento HTML (id="demo") y cambia el contenido del elemento (innerHTML) a "Hola JavaScript":

**Ejemplo:**

```html
document.getElementById("demo").innerHTML = "Hola JavaScript";
```

> **Nota:** JavaScript acepta comillas simples y dobles.👇

**Ejemplo:**

```html
document.getElementById('demo').innerHTML = 'Hola JavaScript';
```

## JS puede cambiar los valores de los atributos

En este ejemplo, JavaScript cambia el valor del atributo src de la etiqueta `<img>`:

**Ejemplo:**

<iframe height="450" style="width: 100%;" scrolling="no" title="JavaScript puede cambiar el valor del atributo HTML" src="https://codepen.io/xantosromero/embed/yLxdGOW?default-tab=result&editable=true&theme-id=dark" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href="https://codepen.io/xantosromero/pen/yLxdGOW">
  JavaScript puede cambiar el valor del atributo HTML</a> por Santos Romero (<a href="https://codepen.io/xantosromero">@xantosromero</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>

## JS puede cambiar los estilos

Cambiar el estilo de un elemento HTML, es una variante de cambiar un atributo HTML.

**Ejemplo:**
```html
document.getElementById("demo").style.fontSize = "35px";
```

## JS puede ocultar elementos

Se pueden ocultar elementos HTML cambiando el estilo `display`.

**Ejemplo:**
```html
document.getElementById("demo").style.display = "none";
```
## JS puede mostrar elementos

También se pueden mostrar elementos HTML ocultos cambiando el estilo `display`.

**Ejemplo:**

```html
document.getElementById("demo").style.display = "block";
```

## ¿Sabías esto?

- JavaScript y Java **son lenguajes completamente diferentes**, tanto en concepto como en diseño.
- JavaScript fue **inventado por Brendan Eich** en 1995 y se convirtió en un estándar ECMA en 1997.
- ECMA-262 es el nombre oficial del estándar. ECMAScript es el nombre oficial del idioma.

## Conclusión

JavaScript puede modificar el contenido HTML con métodos como `getElementById()`, cambiar el texto de un elemento con `innerHTML`. También puede modificar atributos, como el `src` de una imagen, y estilos CSS, como el tamaño de fuente con `style.fontSize`. Además, JavaScript permite ocultar o mostrar elementos cambiando el estilo `display`.
