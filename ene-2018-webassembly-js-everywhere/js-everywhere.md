# Javascript Everywhere

Johny Five - Plataforma para conectar JS con Arduino

```
npm install johny-five
```

Johny five usa node, por lo cual necesita un sistema operativo.
Intel Edison, Raspberry -> se puede usar sin tener que tener el 
aparato conectado al computador

Es necesario recargar el firmware de Arduino para poder utilizar
Johny Five

Se pueden usar los módulos de npm!!

## Ejemplo 1

```js
// hello.js
const jf = require('johny-five');
const board = jf.Board()

board.on('ready', () => {
  const led = new jf.Led(13);

  setInterval(() => {
    led.toggle();
  }, 3000);
});

```

Para correrlo: `node hello.js`

udoo --> 

**Web of Things**

Juan Guillermo Gómez  
fb.com/escueladevhack
