# Primeros Pasos

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

### Declaraciones

Hay tres tipos de declaraciones en JavaScript.

* **var**

    Declara una variable, inizializa opcionalmente un valor.

* **let**

   Declara una variable local en un bloque de ámbito(scope), inicializa opcionalmente un valor. (nuevo en ECMAScript 6)

* **const**

    Declaración de una constante de solo lectura. No provocará un error si se intenta modificar su valor pero no tendrá ningún efecto intentar cambiarlo (nuevo en ECMAScript 6)

Las variables se usan como nombres simbólicos para valores en tu aplicación. Los nombres de las variables, llamados identificadores, se rigen por ciertas reglas.

Un identificador en JavaScript tiene que empezar con una letra, un guión bajo (\_) o un símbolo de dólar ($); los valores subsiguientes puede ser números. Debido a que JavaScript diferencia entre mayúsculas y minúsculas, las letras incluyen tanto desde la "A" hasta la "Z"(mayúsculas) como de la "a" hasta la "z".

Puedes usar la ISO 8859-1 o letras Unicode tales como å y ü en un identificador. Puedes también usar el Unicode escape sequences como caracteres en identificadores.


### Ámbitos de las variable

Son llamadas una variable global si están declaradas fuera de una función, podrá ser utilizada en cualquier parte del documento actual. Son llamadas variables locales si están declaradas dentro de una función, porque estará disponible solo dentro de esa función.

Antes de ECMAScript 6 Javascript no tenía ámbito en los bloques de sentencias. Una variable declarada dentro de un bloque era local para la función (o ámbito global) que el bloque reside dentro. Por ejemplo, el siguiente código registrará 5, porque el ámbito de x es la función(o contexto global) dentro de la cual se declara x, no el bloque, que en este caso es la sentencia if.

~~~
if (true) {
  var a = 5;
}
console.log(a); // 5
~~~

https://developer.mozilla.org/es/docs/Web/JavaScript/Guide/Grammar_and_types
