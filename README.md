# Diplomado de infografia

#### MÓDULO WEB

**Nuestro objetivo**: Reconocer y utilizar los lenguajes que, en la actualidad, son claves en la producción de infografías para soporte digital en línea. Estos lenguajes son: 

- HTML
- CSS
- JavaScript (JS)

Los dos primeros son "lenguajes de descripción", mientras que el tercero es un lenguaje de programación. 

Los dos primeros nos pueden exigir mucha memoria, mientras que el tercero exijirá, además de memoria, mucha lógica.

-------

**¿Por qué podrían exigir la menoria?** Porque determinadas siglas, abreviaciones y palabras, escritas de un único modo, sirven para describir o programar distintas cosas.

Por ejemplo, en **HTML**: 

`<p>Este es un párrafo <span id="especial">con un segmento de identidad especial</span> y un <a href="https://www.google.cl/">vínculo a Google</a></p>`. 

Acá tienen que recordar que `p` es `paragraph`, `span` es un segmento (o lapsus), `id` es `identity`, `a` es `archor` y `href` es `hypertext reference`. Pero siempre se puede contar con herramientas para externas para "memorizar"; [un "torpedo" o "cheat sheet" de HTML5 puede ayudar](https://websitesetup.org/HTML5-cheat-sheet.pdf). 

Otro ejemplo, en **CSS**:

`p{font-family:Helvetica, sans-serif;} span#especial {font-weight:800;} a{color:#f00;} `

Acá notarán que antes del paréntesis de llave hay una referencia al HTML ya presentado, dentro de los mismos paréntesis dice `font-family` para definir la familia de fuente tipográfica que debe usarse en el elemento referido, `font-weight` se usa para definir peso de la fuente, y `color` se usa para definir color (del texto). En este caso también se pueden usar herramientas externas para "memorizar": [CSS3 cheat sheet](https://cloud.netlifyusercontent.com/assets/344dbf88-fdf9-42bb-adb4-46f01eedd629/d7fb67af-5180-463d-b58a-bfd4a220d5d0/css3-cheat-sheet.pdf) 

Un último ejemplo, en **JS**:

`console.log(Math.round(Math.PI))`

En este ejemplo tenemos que aprovechar lo aprendido en álgebra y en aritmética: los paréntesis indican que las operaciones que ellos encierran tienen prioridad ante las demás. O sea, lo primero es explicar que `Math.PI` me entrega el número π, número que necesito redondeado (`Math.round`) para luego imprimirlo en la consolta de JavaScript de navegador (`console.log`). Acá los [torpedos o *cheat sheets* deben ser más extensos](https://htmlcheatsheet.com/js/).

-------

**¿Y por qué podrían exigir la lógica?** Porque programar es escribir un conjunto ordenado y finito de operaciones que permiten hacer algo. Y ya pudieron notar que en el ejemplo anterior aparecieron los "fantasmas" de álgebra y aritmética. 

Ahora pongamos un ejemplo de JS, el único que será necesario cuando este sí es un lenguaje de programación, mientras HTML y CSS sólo son lenguajes descriptivos:

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

Se crea una variable `d`, a la que se le asigna el valor de la fecha en la que se carga el documento (considerando hasta el segundo). Luego, a una variable `h` se le asigna solo la hora en esa fecha. Después se crea una variable con el nombre `saludo`, sin asignarle valor.

Luego vienen unas condiciones (`if (…){…}`, `else if (…){…}`, `else{…}`) en donde se le asigna a la variable `saludo` el valor que corresponda a la hora del día en que se cargue el documento. 

Finalmente, se indica que en el mismo documento cargado se debe escribir el valor de `saludo`, que será el mensaje que corresponda a la hora.
