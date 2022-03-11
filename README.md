# Soy un buen programador JS

Juego con retos sencillos de JavaScript para probarte a ti mismo que sabes lo que haces.

<img src="logo.png" width="250">

## Solo 2 Reglas

1. Todas las variables deben ser constantes. No uses ni `let` ni `var`, solo `const`.
2. Prohibido usar los bucles: `while` y `for`.

## ¿Cómo se entrega?

Crea un Issue y pégame el código. Encantado te daré retroalimentación.

## ✅ Reto 1

Crea un `Array` con números de 0 al 10.

**Solución**: ~~24 de febrero~~ 

Videoexplicación: https://youtu.be/ROijmck2a6w

```javascript
// Forma 1 - La más equilibrada en recursos.
Array(11).fill().map((valor, indice) => indice);

// Forma 2
[...Array(11).keys()]

// Forma 3
Array.from({length: 11}, (v, i) => i);
```

## ✅ Reto 2

A partir del siguiente `Array`.

```javascript
const miLista = [1, 9, 87, 3, 10, 4, 20, 2, 45];
```

Crea una nueva lista con números de 1 digito.

```javascript
// [1, 9, 3, 4, 2];
```

**Solución**: ~~3 de marzo~~ 

Videoexplicación: https://youtu.be/OfUt_BjoGcg

```javascript
const miLista = [1, 9, 87, 3, 10, 4, 20, 2, 45];
const miLista1Decimal = miLista.filter((numero) => /\b-?[0-9]\b/.test(numero));
```

## ✅ Reto 3

A partir del siguiente `Array`.

```javascript
const miLista = ["Lisp", "Clojure", "Haskell", "PHP", "Racket"]
```

Elimina el elemento que se encuentra en la posición 3. Insisto: posición 3, no por el string "PHP".

**Solución**: ~~10 de marzo~~

```javascript
const miLista = ["Lisp", "Clojure", "Haskell", "PHP", "Racket"]

const miListaSinPHP = semana.filter(function(valor, indice) {
    return indice !== 3
});
```

## 🟩 Reto 4

A partir del siguiente `Array`.

```javascript
const miLista = ["Lisp", "Clojure", "Haskell", "Elm", "Racket", "Swift", "Erlang", "Scala"]
```

Obtén el número de elementos que contienen una letra "s" en su valor (o una "s" en su texto).

Si quieres subir el nivel, no uses "length".

**Solución**: 17 de marzo

# ☝🏻 ------ Actuales (Hacer) ------ ☝🏻

Espacio cuantico 📦 🐈

# 👇🏻 ---- Futuras (NO hacer) ------ 👇🏻

## 🟩 Reto 5

Crea una función que elimine los acentos de un `string`. Prohibido usar `Regex` o `replace`.

**Solución**: 24 de marzo

## 🟩 Reto 6

Crea una `Array` que muestre los primeros 10 números de la secuencia de Fibonacci.

¿Subimos el nivel? Crea una función donde le indiques la cantidad de números que quieres en la secuencia.

**Solución**: 31 de marzo

## 🟩 Reto 7

Crea una `Array` con 10 números aleatorios enteros sin que se repitan y estén ordenados de menor a mayor.

**Solución**: 7 de abril

## 🟩 Reto 8

Crea una función que mueva elementos dentro de una `Array`. Por ejemplo, si quisiera mover Scala, que esta en la posición 7, a la posición 1: 

``` javascript
const miLista = ["Lisp", "Clojure", "Haskell", "Elm", "Racket", "Swift", "Erlang", "Scala"]

moverElemento(7, 1, miLista);

// ["Lisp", "Scala", "Clojure", "Haskell", "Elm", "Racket", "Swift", "Erlang"]

```

Como puedes observar, no solo se han intercambiado, sino que el resto de elementos se han movido para hacerle sitio.

**Solución y entrega**: 14 de abril
