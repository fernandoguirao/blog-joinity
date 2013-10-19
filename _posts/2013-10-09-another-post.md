---
layout: post

title: Another post
subtitle: "This is the subtitle"
cover_image: blog-cover.jpg

excerpt: "Cras mattis consectetur purus sit amet fermentum. Cras mattis consectetur purus sit amet fermentum."

author:
  name: Borja de Gregorio
  twitter: fguirao
  gplus: 2323123123 
  bio: CEO
  image: ks.png
---
[ ](http://alfonsomarin.com/wp-content/uploads/2013/04/tutorial-backbone-
js.png)![Tutorial de Backbone.js](http://alfonsomarin.com/wp-content/themes/ev
erest/framework/extensions/timthumb/timthumb.php?src=http%3A%2F%2Falfonsomarin
.com%2Fwp-content%2Fuploads%2F2013%2F04%2Ftutorial-backbone-js.png&w=652)

Llevo un tiempo analizando y aprendiendo a trabajar con la librera
[Backbone.js](http://documentcloud.github.com/backbone/) y me parece una
librera estupenda para desarrollar aplicaciones JavaScript. El mayor problema
que estoy encontrando es la falta de tutoriales y documentacin al respecto, y
por ese motivo he decido crear un pequeo tutorial donde se analice el
funcionamiento de la librera. Este tutorial lo ir desarrollando poco a poco en
distintas entradas, intentando resaltar los aspectos ms importantes y
analizando cada uno de sus componentes.

## Introduccin

Backbone es una excelente librera para construir aplicaciones JavaScript que
nos ofrece la posibilidad de estructurar nuestro cdigo siguiendo el patrn MVC
(Modelo, Vista, Controlador). Como su nombre indica, el objetivo de esta
librera es formar parte de la columna vertebral de nuestra aplicacin
ofrecindonos nicamente la funcionalidad necesaria para que puedas
estructurarla correctamente. De hecho, esa es una de sus grandes virtudes pues
se centra nicamente en proporcionarte conceptos bsicos como modelos, eventos,
colecciones, vistas, routing y persistencia. En tan solo 4KB Backbone
proporciona un marco de trabajo estupendo que podremos utilizar como
complemento a jQuery.

Una librera JavaScript como jQuery es extremadamente til para seleccionar y
modificar elementos del DOM, uso homogneo de AJAX o generacin de efectos y
animaciones, pero a la hora de hacer una aplicacin web de una nica pgina donde
gran parte de la funcionalidad reside en cdigo JavaScript, rpidamente
descubrirs que no es suficiente. En cuanto incluyas ciertas funcionalidades a
tu aplicacin te vers sobrepasado por una gran pila de selectores y callbacks
sin estructura alguna que estarn lidiando directamente con los elementos DOM.

Como veremos, en Backbone los datos los introducimos en **modelos** que
podremos crear, validar, destruir y salvar en el servidor, ofreciendo un
conjunto de **eventos** que se dispararn cuando el modelo cambie. Tambin se
podrn asociar a **vistas** que sern notificadas de dichos cambios para que
puedan actualizar su contenido; agruparemos los modelos en **colecciones** y
podremos implementar las distintas funcionalidades de nuestra aplicacin
utilizando **routers** que nos mapearn distintas rutas de aplicacin con
funciones especficas.

## Descarga y puesta a punto

La nica dependencia que tiene Backbone es
**[underscore.js](http://documentcloud.github.com/underscore/)**, una librera
llena de utilidades y funciones JavaScript de propsito general creada por la
misma gente de Backbone, y entre las funcionalidades que ofrece se encuentran
la manipulacin de arrays, el enlazado de funciones (binding) o templates
JavaScript. Por otra parte, Backbone no realiza ninguna operacin de manejo y
modificacin del DOM o tratamiento de AJAX, por lo que las vistas delegan
dichas funcionalidades a libreras como [jQuery](http://jquery.com/) o
[Zepto.js](http://zeptojs.com/).

Por ese motivo, para la realizacin de los distintos ejemplos de este tutorial
deberamos crear una pgina HTML que se encargase de incorporar todos estos
elementos:

        <</span>script type="text/javascript" src="js/jquery.js">// 
      mce:0
    // ]]>
    
Como podrs imaginar, en el fichero examples.js ser donde vayamos introduciendo
nuestro propio cdigo.

## Partes de este tutorial

Como he comentado al principio, este tutorial lo voy a desarrollar a lo largo
de varias entradas, una por cada tema a tratar. A continuacin os muestro los
distintos temas que abordaremos:

  1. [ Eventos](http://alfonsomarin.com/desarrollo-web/tutoriales/backbonejs-i-eventos)
  2. [ Modelos](http://alfonsomarin.com/desarrollo-web/tutoriales/backbonejs-ii-modelos)
  3. [ Colecciones](http://alfonsomarin.com/desarrollo-web/tutoriales/backbonejs-iii-colecciones)
  4. [ Vistas](http://alfonsomarin.com/desarrollo-web/tutoriales/backbonejs-iv-vistas)
  5. [ Routers](http://alfonsomarin.com/desarrollo-web/tutoriales/backbonejs-v-routers)
  6. [ Sincronizacin y persistencia](http://alfonsomarin.com/desarrollo-web/tutoriales/backbonejs-vi-sincronizacion-y-persistencia)

Al final del tutorial intentar abordar la creacin de una aplicacin completa
que pudiera de servir como ejemplo prctico, pero no me comprometo a ello
![:)](http://alfonsomarin.com/wp-includes/images/smilies/icon_smile.gif)

## Actualizaciones

Este tutorial se basa en la versin 0.5.3 de Backbone. Mi intencin es ir
actualizndolo segn vayan incluyendo nuevas funcionalidades en versiones
posteriores.

19 08 2012 [ Novedades en Backbone 0.9.2](http://alfonsomarin.com/desarrollo-
web/articulos/novedades-en-backbone-0-9-2)

URL[http://alfonsomarin.com/desarrollo-
web/tutoriales/backbonejs](http://alfonsomarin.com/desarrollo-
web/tutoriales/backbonejs)

