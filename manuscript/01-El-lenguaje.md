# El Lenguaje

## javaScript vs ECMAScript

ECMAScript es el nombre oficial de javaScript, porque era necesario encontrar un nombre diferente a la marca registrada _Java_ (Original de Sun y ahora en poder de Oracle). Por lo general todo el mundo hace referencia a javaScript para referirse al lenguaje y a ECMAScript para referirse a la versión. En el momento de escribir este libro ECMAScript se encuentra en su versión 6 y su acrónimo ES6 da nombre a este libro.

## Sintaxis

La sintaxis de JavaScript es muy similar a la de otros lenguajes de programación como Java y C. Las normas básicas que definen la sintaxis de JavaScript son las siguientes:

* _Se pueden incluir comentarios:_ los comentarios se utilizan para añadir información en el código fuente del programa. Aunque el contenido de los comentarios no se visualiza por pantalla, si que se envía al navegador del usuario junto con el resto del script, por lo que es necesario extremar las precauciones sobre la información incluida en los comentarios.
Los comentarios de una sola línea comienzan con //
Los comentarios multilínea se definen encerrando el texto del comentario entre los símbolos /\* y \*/
/\* no puedes, sin embargo, /\* anidar comentarios \*/ SyntaxError \*/

* _No se tienen en cuenta los espacios en blanco y las nuevas líneas:_ como sucede con XHTML, el intérprete de JavaScript ignora cualquier espacio en blanco sobrante, por lo que el código se puede ordenar de forma adecuada para entenderlo mejor (tabulando las líneas, añadiendo espacios, creando nuevas líneas, etc.)

* _Se distinguen las mayúsculas y minúsculas:_ al igual que sucede con la sintaxis de las etiquetas y elementos XHTML. Sin embargo, si en una página XHTML se utilizan indistintamente mayúsculas y minúsculas, la página se visualiza correctamente, siendo el único problema la no validación de la página. En cambio, si en JavaScript se intercambian mayúsculas y minúsculas el script no funciona.

* _No es necesario terminar cada sentencia con el carácter de punto y coma (;):_ en la mayoría de lenguajes de programación, es obligatorio terminar cada sentencia con el carácter ;. Aunque JavaScript no obliga a hacerlo, es conveniente seguir la tradición de terminar cada sentencia con el carácter del punto y coma (;).

https://developer.mozilla.org/es/docs/Web/JavaScript/Guide/Grammar_and_types
