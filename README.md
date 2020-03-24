# PAW2020-TP1-Salinas
 Entrega del trabajo práctico 1 para Programación Web de Luján.

Las consignas de los ejercicios prácticos se encuentran dentro del archivo HTML correspondiente a la resolución.

Respuestas a las preguntas teoricas:


 1. ¿Qué es un lenguaje de marcado? ¿Cuál es su utilidad? ¿Qué es un tag? ¿Qué es un atributo?

Un lenguaje de marcado es una forma de cofificar un documento que, junto con el texto, incorpora etiquetas o marcas que contienen información sobre la estrtuctura del texto y su presentación. Un tag es una marca que delimita una región dentro del documento. Un atributo es un parámetro específico de un dado tag. Cada tag puede poseer muchos atributos.



2. ¿Cuál es la utilidad de HTML? ¿Qué conjunto mínimo de tags debe contener un documento elaborado en este lenguaje? Describa brevemente su utilidad.

El leguaje HTML se utiliza para crear documentos que muestren una estructura de hipertexto. Estos documentos se conforman como documentos de texto plano en los que todo el formato del texto se especifica mediante marcas de texto (tags), los cuales delimitan los contenidos a los que afecta. Dependiendo del contenido de estos tags, los navegadores representarán el texto con un formato determinado.
El conjunto mínimo de tags que debe tener un docomento elaborado en este lenguajes es:

`<!DOCTYPE html>` - indica que el documento está en formato HTML.
`<html lang="es">` - indica el lenguaje utilizado.  En este caso español. Aunque no es una línea obligatoria.
`<body> </body>` - Entre estas etiquetas se define el cuerpo del documento.



3. ¿Cuál es la utilidad e importancia de los enlaces o links entre páginas? ¿Qué significa hipertexto? ¿Un link solo puede apuntar a otra página? ¿Qué importancia tiene esto último?

Los enlaces o links permiten acceder a datos o recursos que no necesariamente se encuentran de forma local en el servidor, y hacerlo de forma transparente desde el punto de vista del usuario.
Hipertexto es un sistema de organización y presentación de los datos en la cual se vinculan fragmentos de un documento con otros documentos, logrando así que el acceso a la información no sea necesariamente secuencial.
Un link no necesariamente debe apuntar a otra página, sino que puede apuntar a distintos tipos de datos tales como imágenes, videos, archivos, etc. La importancia de esto último es la versatilidad y flexibilidad que proporciona a las páginas web.



4. ¿Cómo funcionan los tags audio y video?

`<audio>` es un tag de html5 que permite embeber archivos de audio en una página html. Para ello, el atributo `src` debe contener el path (relativo o absoluto) a un archivo de audio compatible. 
El atributo `controls` agrega controles para la reproducción del audio, tales como botones de play/pausa, control de volumen, barra de progreso, etc.

`<audio src="path" controls></audio>`

Mediante el uso del tag `<source>` se puede especificar diferentes formatos del mismo audio, logrando así que el browser pueda elegir entre varias alternativas. El primer formato reconocido será el seleccionado. Si se incluye texto entre los tags `<audio>` y `</audio>`, éste sólo será visible en caso de que el browser no soporte los elementos `<audio>`

`<audio controls>
	<source src=”path/audio.mp3” type=”audio/mpeg”>
	<source src=”path/audio.ogg” type=”audio/ogg”>
	Tu navegador no soporta los elementos de audio.
</audio>`

`<video>` es un tag html5 que permite embeber archivos de video en una página html. Al igual que con los archivos de audio, el atributo “controls” permite agregar controles para el manejo del video y el tag `<source>` permite agregar distintos formatos para que el browser elija. Es recomendable además incluir siempre los atributos `width` y `height`. Caso contrario la página puede parpadear mientras el video se carga.

`<video width=”320” height=”240” controls>
	<source src=”path/video.mp4” type=”video/mp4”>
	<source src=”path/video.ogg” type=”video/ogg”>
	Tu navegador no soporta los elementos de video.
</audio>`



5. ¿Qué es el Rendering Engine de un Browser? ¿Cuál es el que utiliza cada uno de los 5 browsers más conocidos (Chrome, Firefox, Safari, IE-Edge, Opera)? ¿Cuál es la importancia de conocer cada uno de ellos en la construcción de un sitio?

El Rendering Engine de un browser es un componente central de los browsers. Es el encargado de transformar el texto html en contenido visual para el usuario según el dispositivo en el que se utiliza. 

Engine de los browsers más populares: Blink para Chrome, Edge y Opera; Gecko para Firefox y WebKit para Safari. Anteriormente, Edge utilizaba el motor EdgeHTML y Opera utilizaba el motor Presto.

La importancia de conocer cada uno de ellos en la construcción de un sitio es que la misma página html puede (o no) tener diferencias de visualización dependiendo del navegador. Con lo cual un sitio web que se ve perfectamente en un dado navegador, no necesariamente va a verse de igual modo en otro navegador que utilice un rendering engine diferente. Un sitio web bien diseñado ofrecerá, en caso de ser necesario, diferentes archivos html, css, js, etc., dependiendo del navegador que lo solicita.

