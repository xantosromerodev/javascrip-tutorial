# 

## Las variables son contenedores para almacenar datos

Las variables en JavaScript se pueden declarar de 4 formas:

- Automáticamente
- Usando `var`
- Usando `let`
- Usando `const`

En este primer ejemplo, `x`, `y` y `z` son variables no declaradas.

Se declaran automáticamente cuando se utilizan por primera vez.

**Ejemplo:**
```js
x = 5;
y = 6;
z = x + y;
```

### Nota 1

Se considera una buena práctica de programación declarar siempre las variables antes de usarse.

Del siguiente ejemplo puedes adivinar:

- `x` almacena el valor `5`
- `y` almacena el valor `6`
- `z` almacena el valor `11`

**Ejemplo:**
```js
var x = 5;
var y = 6;
var z = x + y;
```

### Nota 2

La palabra clave `var` se utilizó en todo el código JavaScript desde 1995 hasta 2015.

Las palabras clave `let` y `const` se agregaron a JavaScript en 2015.

La palabra clave `var` sólo debe usarse en código escrito para navegadores más antiguos.


**Ejemplo con `let`:**
```js
let x = 5;
let y = 6;
let z = x + y;
```

**Ejemplo con `const`:**
```js
const x = 5;
const y = 6;
const z = x + y;
```

**Ejemplo mixto:**
```js
const price1 = 5;
const price2 = 6;
let total = price1 + price2;
```

Las dos variables `price1` y `price2` se declaran con la palabra clave `constv.

Estos son valores constantes y no se pueden cambiar.

La variable total se declara con la palabra clave `let`.

El valor de la variable `total` puede cambiar.

### ¿Cuándo utilizar `var`, `let` o `const`?

1. Siempre declare variables.
2. Siempre utilice `const` si el valor no va cambiar.
3. Siempre utilice `const` si no va cambiar el tipo (matrices y objetos).
4. Solo usa `let` si no puedes usar `const`.
5. Utilice `var` únicamente si DEBES codificar para navegadores antiguos.

## Como en el álgebra

Al igual que en álgebra, las variables contienen valores:

```js
let x = 5;
let y = 6;
```

Al igual que en álgebra, las variables se utilizan en expresiones:
```js
let z = x + y;
```

A partir del ejemplo anterior, puedes adivinar que el total calculado es 11.

> **Nota:** Las variables son contenedores para almacenar valores.

## Identificadores JavaScript

Todas las **variables** de JavaScript deben **identificarse** con **nombres únicos**.

Estos nombres únicos se denominan **identificadores**.

Los identificadores pueden ser nombres cortos (como `x` y `y`) o nombres más descriptivos (edad, suma, volumenTotal).

Las reglas generales para crear nombres de variables (identificadores únicos) son:

- Los nombres pueden contener letras, dígitos, guiones bajos y signos de dólar.
- Los nombres deben comenzar con una letra.
- Los nombres también pueden comenzar con $_ (pero no lo usaremos en este tutorial).
- Los nombres distinguen entre mayúsculas y minúsculas (`y` y `Y` son variables diferentes).
- Las palabras reservadas (como las palabras clave de JavaScript) no se pueden utilizar como nombres de variables.

> **Nota:** Los identificadores JavaScript distinguen entre mayúsculas y minúsculas.

## El operador de asignación

En JavaScript, el signo igual (`=`) es un operador de "asignación", no un operador "igual a".

Esto es diferente del álgebra. El siguiente ejemplo no tiene sentido en álgebra:

```js
x = x + 5
```

Sin embargo, en JavaScript, tiene mucho sentido: asigna el valor de `x` + `5`  `x`.

(Calcula el valor de `x` + `5` y coloca el resultado en `x`. El valor de `x` se incrementa en `5`).

> **Nota:** El operador "igual a" se escribe así `==` en JavaScript.

## Tipos de datos JavaScript

Las variables de JavaScript pueden contener números y valores de texto.

En programación, los valores de texto se denominan cadenas de texto.

JavaScript puede manejar muchos tipos de datos, pero por ahora, sólo piense en números y cadenas de texto.

Las cadenas se escriben entre comillas dobles o simples. Los números se escriben sin comillas.

Si pones un número entre comillas, será tratado como una cadena de texto.

**Ejemplo:**
```js
const pi = 3.14;
let persona = "John Doe";
let rpta = 'Si, soy yo';
```

## Declarar una variable

Crear una variable en JavaScript se llama "declarar" una variable.

Declaras una variable JavaScript con la palabra clave `var` o `let`:

```js
var carName;
```

```js
let carName;
```

Después de ser declarado, la variable no tiene valor (técnicamente no está definida).

Para **asignar** un valor a la variable, use el signo igual:

```js
carName = "Volvo";
```

También puedes asignar un valor a la variable cuando la declaras:

```js
let carName = "Volvo";
```

En el siguiente ejemplo, creamos una variable llamada `carName` y le asignamos el valor "Volvo".

Luego "generamos" el valor dentro de un párrafo HTML con `id="demo"`:

**Ejemplo:**
```js
<p id="demo"></p>

<script>
    let carName = "Volvo";
    document.getElementById("demo").innerHTML = carName;
</script>
```

> **Nota:** Es una buena práctica de programación declarar todas las variables al comienzo de un script.

## Una declaración, muchas variables

Puedes declarar muchas variables en una sola declaración.

Comienza la declaración con `let` y separe las variables con una **coma**.

**Ejemplo:**
```js
let person = "John Doe", carName = "Volvo", price = 200;
```

Una declaración puede abarcar varias líneas:

**Ejemplo:**
```js
let person = "John Doe",
carName = "Volvo",
price = 200;
```

## Valor = indefinido

En los programas de computadora, las variables a menudo se declaran sin valor. El valor puede ser algo que deba calcularse o algo que se proporcionará más adelante, como la entrada del usuario.

Una variable declarada sin valor tendrá el valor `undefined`.

La variable `carName` tendrá el valor `undefined` después de la ejecución de esta declaración.


**Ejemplo:**
```js
let carName;
```

## Volver a declarar variables JavaScript

Si vuelves a declarar una variable JavaScript declarada con `var`, este no perderá su valor.

La variable `carName` seguirá teniendo el valor "Volvo" después de la ejecución de estas declaraciones.

**Ejemplo:**
```js
var carName = "Volvo";
var carName;
```

### Nota 

No puedes volver a declarar una variable declarada con let o const.

Esto no funcionará:👇

```js
let carName = "Volvo";
let carName;
```

## Aritmética de JavaScript

Al igual que con el álgebra, puedes hacer aritmética con variables de JavaScript, usando operadores como `=` y `+`:

**Ejemplo:**
```js
let x = 5 + 2 + 3;
```

También puedes agregar cadenas, pero las cadenas estarán concatenadas:

**Ejemplo:**
```js
let x = "John" + " " + "Doe";
```

Prueba también esto:

**Ejemplo:**
```js
let x = "5" + 2 + 3;
```

### Nota

Si pone un número entre comillas, el resto de los números se tratarán como cadenas y se concatenarán.

Ahora prueba esto:

**Ejemplo:**
```js
let x = 2 + 3 + "5";
```

## Signo de dólar JavaScript

Dado que JavaScript trata un signo de dólar como una letra, los identificadores que contienen $ son nombres de variables válidos:

**Ejemplo:**
```js
let $ = "Hola Mundo";
let $$$ = 2;
let $myMoney = 5;
```

El uso del signo de dólar no es muy común en JavaScript, pero los programadores profesionales suelen utilizarlo como alias para la función principal en una biblioteca de JavaScript.

En la biblioteca JavaScript jQuery, por ejemplo, la función principal `$` se utiliza para seleccionar elementos HTML. En jQuery `$("p");` significa "seleccionar todos los p elementos".

## Subrayado en JavaScript

Dado que JavaScript trata el guión bajo como una letra, los identificadores que contienen `_` son nombres de variables válidos:

**Ejemplo:**
```js
let _lastName = "Johnson";
let _x = 2;
let _100 = 5;
```

El uso del guión bajo no es muy común en JavaScript, pero una convención entre los programadores profesionales es usarlo como alias para variables "privadas (ocultas)".

## Conclusión

En JavaScript, las variables almacenan datos y se pueden declarar con `var`, `let`, o `const`. `var` es obsoleto, mientras que `let` y `const` son preferibles. Las variables deben tener identificadores únicos y pueden contener números o cadenas de texto. Es importante declarar variables antes de usarlas y seguir buenas prácticas.

