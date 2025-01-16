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



