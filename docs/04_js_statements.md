# Declaraciones JavaScript

**Ejemplo:**
```html
let x, y, z;    // Declaracion 1
x = 5;          // Declaracion 2
y = 6;          // Declaracion 3
z = x + y;      // Declaracion 4
```

## Programas JavaScript

Un **programa de computadora** es una lista de "instrucciones" que una computadora debe "ejecutar".

En un lenguaje de programación, estas instrucciones de programación se denominan declaraciones.

Un **programa JavaScript** es una lista de **declaraciones** de programación.

> En HTML, los programas JavaScript los ejecuta el navegador web.

## Declaraciones JavaScript

Las declaraciones de JavaScript se componen de:

- Valores
- Operadores
- Expresiones
- Palabras clave y comentarios

👇Esta declaración le dice al navegador que escriba "Hola Doly." dentro de un elemento HTML con `id="demo"`.

**Ejemplo:**
```html
<script>
    document.getElementById("demo").innerHTML = "Hola Doly.";
</script>
```

La mayoría de los programas JavaScript contienen muchas declaraciones.

Las declaraciones se ejecutan, una por una, en el mismo orden en que están escritas (de arriba hacia abajo).

> Los programas JavaScript (y las declaraciones JavaScript) a menudo se denominan código JavaScript.

## Punto y coma

El punto y coma separa las declaraciones de JavaScript.

Agregue un punto y coma al final de cada declaración ejecutable.

**Ejemplo:**
```html
let a, b, c;  // Declara 3 variables
a = 5;        // Asigna el valor 5 -> a
b = 6;        // Asigna el valor 6 -> b
c = a + b;    // Asigna la suma de a y b -> c
```

Cuando están separados por punto y coma, se permiten varias declaraciones en una línea.

**Ejemplo:**
```html
a = 5; b = 6; c = a + b;
```

> En la web, es posible que vea ejemplos sin punto y coma. No es obligatorio terminar las declaraciones con punto y coma, pero es muy recomendable.

## Espacios en blanco

JavaScript ignora múltiples espacios. Puedes agregar espacios en blanco al script para hacerlo más legible.

Las siguientes líneas son equivalentes:

```html
let person = "Hege";
let person="Hege";
```

Una buena práctica es poner espacios alrededor de los operadores `(= + - * /)`:

```html
let x = y + z;
```

## Longitud y saltos de línea

Para una mejor legibilidad, los programadores suelen evitar líneas de código de más de 80 caracteres.

Si una declaración de JavaScript no cabe en una línea, el mejor lugar para dividirla es después de un operador.

**Ejemplo:**
```html
document.getElementById("demo").innerHTML =
"Hola Doly";
```

## Bloques de código

Las declaraciones de JavaScript se pueden agrupar en bloques de código, dentro de llaves `{...}`.

El propósito de los bloques de código es definir declaraciones que se ejecutarán juntas.

Un lugar donde encontrará declaraciones agrupadas en bloques es en las funciones de JavaScript.

**Ejemplo:**
```html
function myFunction() {
  document.getElementById("demo1").innerHTML = "Hola Doly!";
  document.getElementById("demo2").innerHTML = "¿Cómo estás?";
}
```

> En este tutorial utilizamos 2 espacios de sangría para bloques de código. Aprenderás más sobre las funciones más adelante en este tutorial.

## Palabras clave

Las declaraciones de JavaScript suelen comenzar con una palabra clave para identificar la acción de JavaScript que se realizará.

Nuestra [referencia de palabras reservadas](https://www.w3schools.com/js/js_reserved.asp) enumera todas las palabras clave de JavaScript.

Aquí hay una lista de algunas de las palabras clave que aprenderás en este tutorial.

| Palabra clave | Descripción |
|-----------|-----------|
| `var` | Declara una variable. |
| `let` | Declara una variable de bloque. |
| `const` | Declara un bloque constante. |
| `if` | Marca un bloque de declaraciones que se ejecutarán bajo una condición. |
| `switch` | Marca un bloque de sentencias para ser ejecutadas en diferentes casos. |
| `for` | Marca un bloque de declaraciones para ejecutar en un bucle. |
| `function` | Declara una función. |
| `return` | Retorna de una función. |
| `try` | Implementa el manejo de errores en un bloque de declaraciones.. |

> Las palabras clave de JavaScript son palabras reservadas. Las palabras reservadas no se pueden utilizar como nombres de variables.

## Conclusión

Un programa JavaScript es una serie de declaraciones que el navegador ejecuta para realizar tareas específicas. Estas declaraciones pueden incluir valores, operadores, expresiones, palabras clave y comentarios. En JavaScript, el punto y coma separa las declaraciones, aunque su uso no es obligatorio, es recomendable. Los bloques de código se agrupan con llaves `{}` y se utilizan en funciones para ejecutar varias declaraciones. Las palabras clave como `var`, `let`, `const`, `if`, `for` y `function` son fundamentales en la programación JavaScript.
