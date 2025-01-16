# Sintáxis de JavaScript

La sintaxis de JavaScript es el conjunto de reglas sobre cómo se construyen los programas en JavaScript.

```js
// Como crear variables:
var x;
let y;

// Como usar variables:
x = 5;
y = 6;
let z = x + y;
```

## Valores JavaScript

La sintaxis de JavaScript define dos tipos de valores:

- Valores fijos
- Valores variables

Los valores fijos se llaman **literales**.

Los valores de las variables se denominan **variables**.

## Literales JavaScript

Las dos reglas de sintaxis más importantes para valores fijos son.

1. Los **números** se escriben con o sin decimales:
```js
10.50

1001
```
2. Las **cadenas son texto**, escrito entre comillas dobles o simples:
```js
"John Doe"

'John Doe'
```

## Variables JavaScript

En un lenguaje de programación, las **variables** se utilizan para **almacenar** valores de datos.

JavaScript utiliza las palabras clave `var`, `let` y `const` para **declarar** variables.

Se utiliza un **signo igual** para **asignar valores** a las variables.

En este ejemplo, `x` se define como una variable. Entonces, a `x` se le asigna (dado) el valor `6`:

```js
let x;
x = 6;
```

## Operadores JavaScript

JavaScript utiliza **operadores aritméticos** ( + - * / ) para **calcular** valores:

```js
(5 + 6) * 10
```

JavaScript utiliza un **operador de asignación** ( = ) para **asignar** valores a variables:

```js
let x, y;
x = 5;
y = 6;
```

## Expresiones JavaScript

Una expresión es una combinación de valores, variables y operadores, que calcula un valor.

El cálculo se llama evaluación.

Por ejemplo, 5 * 10 se evalúa como 50:
```js
5 * 10
```

Las expresiones también pueden contener valores variables:
```js
x * 10
```

Los valores pueden ser de varios tipos, como números y cadenas.

Por ejemplo, "John" + " " + "Doe", se evalúa como "John Doe":
```js
"John" + " " + "Doe"
```

## Palabras clave JavaScript

Las **palabras clave** de JavaScript se utilizan para identificar las acciones que se realizarán.

La palabra clave `let` le dice al navegador que cree variables:
```js
let x, y;
x = 5 + 6;
y = x * 10;
```

La palabra clave `var` también le dice al navegador que cree variables:
```js
var x, y;
x = 5 + 6;
y = x * 10;
```

> En estos ejemplos, usar `var` o `let` producirá el mismo resultado. Aprenderás más sobre `var` y `let` más adelante en este tutorial.

## Comentarios JavaScript

No todas las declaraciones de JavaScript se "ejecutan".

El código después de las barras dobles // o entre /* y */ se tratan como un **comentario**.

Los comentarios se ignoran y no se ejecutarán:
```js
let x = 5;   // Se ejecutará

// x = 6;   No se ejecutará
```

> Aprenderás más sobre los comentarios en un capítulo posterior.

## Identificadores JavaScript

Los identificadores son nombres de JavaScript.

Los identificadores se utilizan para nombrar variables, palabras clave y funciones.

Las reglas para los nombres legales son las mismas en la mayoría de los lenguajes de programación.

Un nombre JavaScript debe comenzar con:

- Una letra (A-Z o a-z)
- Un signo de dólar ($)
- Un guión bajo (_)

Los caracteres siguientes pueden ser letras, dígitos, guiones bajos o signos de dólar.

> **Nota**: No se permiten números como primer caracter en los identificadores. De esta forma, JavaScript puede distinguir fácilmente los identificadores de los números.

## JavaScript es case-sensitive

Todos los identificadores de JavaScript **distinguen** entre **mayúsculas y minúsculas**.

Las variables `lastName` y `lastname`, son dos variables diferentes:

```js
let lastname, lastName;
lastName = "Doe";
lastname = "Peterson";
```

JavaScript no interpreta **LET** o **Let** como la palabra clave **let**.

## JavaScript y Camel Case

Históricamente, los programadores han utilizado diferentes formas de unir varias palabras en un nombre de variable:

**Guiones:**

first-name, last-name, master-card, inter-city

> Los guiones no están permitidos en JavaScript. Están reservados para operaciones de resta.

**Guiones bajo:**

first_name, last_name, master_card, inter_city

**Mayúsculas Camel Case:**

FirstName, LastName, MasterCard, InterCity

**Minúsculas Camel Case:**

Los programadores de JavaScript tienden a utilizar mayúsculas y minúsculas que comienzan con una letra minúscula:

firstName, lastName, masterCard, interCity

## Charset JavaScript

JavaScript utiliza el conjunto de caracteres Unicode.

Unicode cubre (casi) todos los caracteres, puntuaciones y símbolos del mundo.

Para saber más, visita el artículo [Complete Unicode Rerefence](https://www.w3schools.com/charsets/ref_html_utf8.asp).

## Conclusión

Aprendimos la sintáxis de JavaScript, cómo declarar y usar las variables, los tipos de valores literales y variables, y el uso de operadores y expresiones. También aprendimos el uso de las palabras clave `var`, `let`, y `const`, así como el manejo de los comentarios, identificadores y case-sensitive.