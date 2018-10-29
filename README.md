# Diplomado de infografia
### Escuela de Diseño / Pontificia Universidad Católica de Chile / 2018

### MÓDULO WEB

**El objetivo**: Reconocer y utilizar los lenguajes que, en la actualidad, son claves en la producción de infografías para soporte digital en línea. Estos lenguajes son: 

- [HTML](https://github.com/profesorfaco/infografia/wiki/HTML)
- [CSS](https://github.com/profesorfaco/infografia/wiki/CSS)
- [JavaScript (JS)](https://github.com/profesorfaco/infografia/wiki/JS)

Los dos primeros son "lenguajes de descripción", mientras que el tercero es un lenguaje de programación. Los dos primeros nos pueden exigir mucha memorización, mientras que el tercero exigirá, además, mucha lógica.

-------

#### ¿Por qué podrían exigir memorización? 

Porque determinadas siglas, abreviaciones y palabras, escritas de un único modo, sirven para describir o programar determinadas cosas.

**Un ejemplo, en HTML**: 

`<p>Este es un párrafo <span id="especial">con un segmento de identidad especial</span> y un <a href="https://www.google.cl/">vínculo a Google</a></p>`. 

Acá la memoria les puede ayudar a decir que `p` es `paragraph`, `span` es un segmento (o lapsus), `id` es `identity`, `a` es `anchor` y `href` es `hypertext reference`. Hay muchísimo más por memorizar, pero hay "herramientas externas" que pueden ayucar: como [un *torpedo* o *cheat sheet* de HTML5](https://websitesetup.org/HTML5-cheat-sheet.pdf).

**Otro ejemplo, en CSS**:

`p{font-family:Helvetica, sans-serif;} span#especial {font-weight:800;} a{color:#f00;} `

Acá pueden notar que antes de cada paréntesis de llave hay referencias al ejemplo ya presentado (HTML). Dentro de los paréntesis dice `font-family: …` para definir la familia de fuente tipográfica que debe usarse en el elemento referido, `font-weight: …` para definir peso de la fuente, y `color: …` para definir color (del [hiper]texto). 

En este caso también se pueden usar "herramientas para memorizar": [CSS3 cheat sheet](https://cloud.netlifyusercontent.com/assets/344dbf88-fdf9-42bb-adb4-46f01eedd629/d7fb67af-5180-463d-b58a-bfd4a220d5d0/css3-cheat-sheet.pdf) 

**Y un último ejemplo, en JS**:

`console.log(Math.round(Math.PI))`

En este ejemplo pueden aprovechar lo aprendido en álgebra y aritmética: los paréntesis indican que las operaciones que ellos encierran tienen prioridad ante las demás. O sea, lo primero es explicar que `Math.PI` entrega el número π, número que se redondea (`Math.round`) para luego imprimirlo en la [consola de JavaScript de navegador](https://norfipc.com/inf/como-usar-consola-javascript-navegador-web.php) (`console.log`). 

Acá los [torpedos o *cheat sheets* deben ser más extensos](https://htmlcheatsheet.com/js/).

-------

#### ¿Y por qué podrían exigir lógica? 

Porque programar es escribir, en cierto lenguaje, un conjunto ordenado y finito de operaciones que permiten hacer algo.

**Revisemos un ejemplo de JS, el único que será necesario al referirnos a la lógica, cuando es el único lenguaje de programación entre los tres** que se presentan como claves en la producción de infografías para soporte digital en línea. 

```
var d = new Date();
var h = d.getHours();
var saludo;
if ((h >= 6) && (h < 12)) { 
  saludo = "buenos días"
} else if ((h >= 12) && (h < 21)) {
  saludo = "buenas tardes"
} else { 
  saludo = "buenas noches"
}
document.write(saludo);
```

En el ejemplo [se crea una variable](https://github.com/profesorfaco/infografia/wiki/JS-:-variables) `d`, a la que se le asigna almacenar el dato de la fecha en la que [el cliente](https://es.wikipedia.org/wiki/Cliente_(inform%C3%A1tica)) carga la página web (considerando hasta los segundos). Luego, a una variable `h` se le asigna solo la hora en esa fecha. Después se crea una variable con el nombre `saludo`, y no se le asigna dato para almacenar de forma inmediata.

Mediante [condiciones](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/if...else) (`if (…){…}`, `else if (…){…}`, `else{…}`) se le asigna a la variable `saludo` almacenar la cadena de caracteres que corresponda a la hora en que se carga la página web. 

Finalmente, se escribe el valor de `saludo` en el [Document Object Model o DOM](https://www.w3schools.com/js/js_htmldom.asp) de la página web ya cargada.

-----------

**Como el objetivo es reconocer y utilizar tres languajes ([HTML](https://github.com/profesorfaco/infografia/wiki/HTML), [CSS](https://github.com/profesorfaco/infografia/wiki/CSS), [JS](https://github.com/profesorfaco/infografia/wiki/JS)), este módulo será práctico-teórico; en este repositorio podrán encontrar documentos que facilitarán la práctica y [un wiki](https://github.com/profesorfaco/infografia/wiki) que reforzará lo teórico.** 

Todo lo que encuentren en este repositorio es redactado y compartido por **Felipe** **A**lberto **Cortez** **O**rellana, alias [FACO](http://profesor.faco.cl/), Profesor Adjunto de la Universidad de Chile y Profesor Asistente Adjunto de la Pontificia Universidad Católica de Chile.

profesor@faco.cl
