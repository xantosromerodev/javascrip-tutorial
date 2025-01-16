# JavaScript Let

La palabra clave `let` se introdujo en ES6 (2015).

Las variables definidas con `let` tienen **alcance de bloque**.

Las variables definidas con `let` deben **declararse** antes de su uso.

Las variables definidas con `let` no se pueden volver a declarar.

## Alcance de bloque

Antes de ES6 (2015), JavaScript no tenía **alcance de bloque**.

JavaScript tenía **alcance global** y **alcance de función**.

ES6 introdujo dos nuevas palabras clave de JavaScript: `let` y `const`.

Estas dos palabras clave proporcionaban **alcance de bloque** en JavaScript.

**Ejemplo:**

No se puede acceder a las variables declaradas dentro de un bloque { } desde fuera del bloque:

```js
{
  let x = 2;
}
// x NO puede ser usado aquí
```

## Alcance global

Las variables declaradas con la palabra clave `var` siempre tienen un **alcance global**.

Las variables declaradas con la palabra clave `var` NO pueden tener alcance de bloque.

**Ejemplo:**

Las variables declaradas con `var` dentro de un bloque `{ }` pueden ser accedidas desde fuera del bloque.

```js
{
  var x = 2;
}
// x SI se puede usar aquí
```

## No se puede re-declarar

Las variables definidas con `let` no se pueden redeclarar.

No puedes redeclarar accidentalmente una variable declarada con `let`.

Con `let` **no puedes hacer** esto:
```js
let x = "John Doe";

let x = 0;
```

Las variables definidas con `var` **pueden** volver a declararse.

Con `var` **sí puedes** hacer esto:
```js
var x = "John Doe";

var x = 0;
```

## Redeclarando variables

Redeclarar una variable utilizando la palabra clave `var` puede causar problemas.

Redeclarar una variable dentro de un bloque también redeclarará la variable fuera del bloque.

**Ejemplo:**
```js
var x = 10;
// Aquí x es 10

{
var x = 2;
// Aquí x es 2
}

// Aquí x es 2
```

Redeclarar una variable utilizando la palabra clave `let` puede solucionar este problema.

Redeclarar una variable dentro de un bloque no redeclarará la variable fuera del bloque.

**Ejemplo:**
```js
let x = 10;
// Aquí x es 10

{
let x = 2;
// Aquí x es 2
}

// Aquí x es 10
```

## Diferencias entre `var`, `let` y `const`

|  | Alcance | Redeclarar | Reasignar | Hoisting | Enlazar |
|-----------|-----------|-----------|-----------|-----------|-----------|
| `var`    | No    | Si   | Si   | Si    | Si    |
| `let`    | Si    | No     | Si   | No     | No     |
| `const`  | Si   | No    | No     | No     | No   |

## ¿Cuál es mejor?

`let` y `const` tienen **alcance de bloque**.

`let` y `const` no se pueden **redeclarar**.

`let` y `const` deben ser **declarados** antes de su uso.

`let` y `const` no se **enlazan** a `this`.

`let` y `const` no son **elevados** (hoisted).

## ¿Cuál no es bueno?

`var` no tiene que ser declarada.

`var` es elevada (hoisted).

`var` se enlaza a `this`.

## Soporte con el navegador

Las palabras clave `let` y `const` no son compatibles con Internet Explorer 11 o versiones anteriores.

La siguiente tabla define las primeras versiones de los navegadores con soporte completo:

| Chrome 49 | Edge 12 | Firefox 36 | Safari 11	 | Opera 36 |
|-----------|-----------|-----------|-----------|-----------|
| Mar, 2016   | Jul, 2015    | Jan, 2015   | Sep, 2017   | Mar, 2016   |

## Redeclarando

Redeclarar una variable de JavaScript con `var` está permitido en cualquier parte de un programa.

**Ejemplo:**
```js
var x = 2;
// Ahora x es 2

var x = 3;
// Ahora x es 3
```

Con `let`, no se permite redeclarar una variable en el mismo bloque.

**Ejemplo:**
```js
var x = 2;   // Permitido
let x = 3;   // No permitido

{
let x = 2;   // Permitido
let x = 3;   // No permitido
}

{
let x = 2;   // Permitido
var x = 3;   // No permitido
}
```

Redeclarar una variable con `let` en otro bloque SÍ está permitido.

**Ejemplo:**
```js
let x = 2;   // Permitido

{
let x = 3;   // Permitido
}

{
let x = 4;    // Permitido
}
```

## Let Hoisting

Las variables definidas con `var` son elevadas (hoisted) al principio y pueden ser inicializadas en cualquier momento.

Esto significa que puedes usar la variable antes de que sea declarada.

**Ejemplo:**
Esto está bien.
```js
carName = "Volvo";
var carName;
```

Si deseas aprender más sobre hoisting, estudia el capítulo sobre [Hoisting en JavaScript](https://www.w3schools.com/js/js_hoisting.asp).

Las variables definidas con `let` también son elevadas (hoisted) al principio del bloque, pero no se inicializan.

Esto significa que usar una variable `let` antes de ser declarada resultará en un `ReferenceError`.

**Ejemplo:**
```js
carName = "Saab";
let carName = "Volvo";
```

## Conclusión

En este capítulo, hemos explorado el uso de la declaración `let` en JavaScript. A diferencia de `var`, `let` permite declarar variables con un alcance de bloque, lo que ayuda a evitar errores comunes relacionados con el alcance de las variables. También hemos visto que las variables declaradas con `let` no pueden ser redeclaradas en el mismo ámbito y que intentar usar una variable `let` antes de su declaración resultará en un `ReferenceError`. Estos comportamientos hacen que `let` sea una opción más segura y predecible para declarar variables en JavaScript.
