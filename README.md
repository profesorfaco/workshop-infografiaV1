# Diplomado de infografia
#### Escuela de Diseño / Pontificia Universidad Católica de Chile / 2018

### MÓDULO WEB

**Nuestro objetivo**: Reconocer y utilizar los lenguajes que, en la actualidad, son claves en la producción de infografías para soporte digital en línea. Estos lenguajes son: 

- HTML
- CSS
- JavaScript (JS)

Los dos primeros son "lenguajes de descripción", mientras que el tercero es un lenguaje de programación. Los dos primeros nos pueden exigir mucha memorización, mientras que el tercero exigirá, además, mucha lógica.

-------

**¿Por qué podrían exigir memorización?** Porque determinadas siglas, abreviaciones y palabras, escritas de un único modo, sirven para describir o programar determinadas cosas.

Por ejemplo, en **HTML**: 

`<p>Este es un párrafo <span id="especial">con un segmento de identidad especial</span> y un <a href="https://www.google.cl/">vínculo a Google</a></p>`. 

Acá tienen que memorizar que `p` es `paragraph`, `span` es un segmento (o lapsus), `id` es `identity`, `a` es `anchor` y `href` es `hypertext reference`. Pero siempre se puede contar con "herramientas para memorizar", como [un "torpedo" o "cheat sheet" de HTML5](https://websitesetup.org/HTML5-cheat-sheet.pdf), o confiando en lo que va mostrándote como opciones el software de edición de código.

Otro ejemplo, en **CSS**:

`p{font-family:Helvetica, sans-serif;} span#especial {font-weight:800;} a{color:#f00;} `

Acá notarán que antes de cada paréntesis de llave hay referencias al ejemplo ya presentado (HTML). Dentro de los paréntesis dice `font-family: …` para definir la familia de fuente tipográfica que debe usarse en el elemento referido, `font-weight: …` para definir peso de la fuente, y `color: …` para definir color (del texto). En este caso también se pueden usar "herramientas para memorizar": [CSS3 cheat sheet](https://cloud.netlifyusercontent.com/assets/344dbf88-fdf9-42bb-adb4-46f01eedd629/d7fb67af-5180-463d-b58a-bfd4a220d5d0/css3-cheat-sheet.pdf) 

Un último ejemplo, en **JS**:

`console.log(Math.round(Math.PI))`

En este ejemplo tenemos que aprovechar lo aprendido en álgebra y aritmética: los paréntesis indican que las operaciones que ellos encierran tienen prioridad ante las demás. O sea, lo primero es explicar que `Math.PI` me entrega el número π, número que necesito redondeado (`Math.round`) para luego imprimirlo en la [consola de JavaScript de navegador](https://norfipc.com/inf/como-usar-consola-javascript-navegador-web.php) (`console.log`). Acá los [torpedos o *cheat sheets* deben ser más extensos](https://htmlcheatsheet.com/js/).

-------

**¿Y por qué podrían exigir lógica?** Porque programar es escribir, en cierto lenguaje, un conjunto ordenado y finito de operaciones que permiten hacer algo.

Ahora pongamos un ejemplo de JS, el único que será necesario cuando es el único lenguaje de programación entre los tres que se presentan como claves en la producción de infografías para soporte digital en línea. 

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

Se crea una variable `d`, a la que se le asigna el valor de la fecha en la que se carga la página web (considerando hasta horas, minutos y segundos). Luego, a una variable `h` se le asigna solo la hora en esa fecha. Después se crea una variable con el nombre `saludo`, sin asignarle valor.

Luego vienen unas condiciones (`if (…){…}`, `else if (…){…}`, `else{…}`) en donde se le asigna a la variable `saludo` el valor que corresponda a la hora en que se cargue el documento. 

Finalmente, se escribe el valor de `saludo` en el [Document Object Model o DOM](https://www.w3schools.com/js/js_htmldom.asp) de la página web ya cargada.

-----------

Como el objetivo es reconocer y utilizar estos languajes (HTML, CSS, JS), la clase será práctica-teórica; en este repositorio podrán encontrar documentos que aportarán a la práctica y un wiki que refozará lo teórico. 

Todo lo que encuentras en este repositorio fue redactado y compartido por **Felipe** **A**lberto **Cortez** **O**rellana, alias [FACO](http://profesor.faco.cl/), a quien pueden contactar con el correo: profesor@faco.cl
