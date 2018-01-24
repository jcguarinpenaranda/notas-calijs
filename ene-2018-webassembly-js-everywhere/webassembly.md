# WebAssembly = wasm

Felipe Janer  
@5h1rU

Excribir código en lenguajes de programación diferentes a Javascript, como C/C++ y Rust

C/C++ o Rust > IR* (bitcode) > wasm > ARM /x86

Esto es un estándar de W3C

## ¿Qué no es?
- NO es un reemplazo de Javascript
- No es una nueva forma de hacer desarrollo web desde cero
- No es un transpiler

Hay 3 formas de hacer que un código funcione

- **Interpretador**: Lee línea por línea y va arrojando los resultados
- **Compilador**: Toma todo el código y genera un binario
- **JIT**: Just in Time. Mezcla Compilador e Intérprete. Optimiza el código a medida que el programa pasa por algunas partes del código. El problema es que JS no es tipado.

Web Assembly no tiene garbage collector, que es quien libera el espacio que no se está usando en la memoria para dejar espacio libre.

## Ventajas

* VideoStreaming puede ser más rápido
* Decodificar es más rápido
* No se complica con los tipos de variables
* Al no tener Garbage Collector, el manejo de la memoria se hace manualmente
* Significa mejoras en el consumo de batería y de procesamiento

Es más rápido porque está más cerca del código máquina

## Utilización con webpack
rust-native-wasm-loader

```js
import('./src/lib.rs').then(wasm => {
  console.log(wasm.add_one(3,4));
});
```

RUST tiene su package manager (Cargo). En la encuesta de StackOverflow es uno de los que más gustan.

## Redes a seguir
@wycats  
@5h1rU
