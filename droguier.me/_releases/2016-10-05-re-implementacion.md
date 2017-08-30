---
title: "Re-Implementación: +Debug+JekyllServe"
modified: 2016-10-05T00:00:00-00:00
---

Un avance mayor para mi página, he implementado el debuger propio de _Jekyll_, el que permite estar probando los cambios que se realizan sobre el sitio desde mi propio ordenador e instantáneamente; para tener una idea clara de la implementación inicial, esta página está ligada al **fork** inicial de _MMistake_, por lo tanto, se implementaba directamente con _GitHub_, lo cual era muy bueno para trabajar, y el proceso de CRUD era:

* Modificar archivos.
* Crear el _pull_.
* Subir modificaciones.

<!--more-->

El proceso no es complejo, pero requiere tiempo para validar los cambios, y si estos fallaban te mostraba la información la consola del error, pero era rehacer el proceso con las nuevas modificaciones.

<!--more-->

Con esta nueva implementación, es posible crear un servidor virtual en el mismo equipo, sin poseer ninguna herramienta adicional como _XAMP_, tan solo ejecutamos **_"jekyll serve"_** o **_"bundle exec jekyll serve"_**, y automáticamente nos genera un servidor para visualizar la página en la dirección **_127.0.0.1:4000_** (es posible modificar el puerto), adicional cuenta con monitor de cambios que al aplicar alguna modificación en alguno de los archivos, inmediatamente regenera la página y te permite visualizar los cambios inmediatamente.

<figure class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/images/releases/probando_con_jekyll_serve.png" alt="">
  <figcaption>Imagen de pantalla de <i>Jekyll Serve</i>.</figcaption>
</figure>

## Eventos registrados:

* Actualizar _Bundle GEM_
* Descargar _Jekyll_ desde _GEM_
* Descargar _MMistake_ desde archivo
* Agregar archivos de boostrap
* Configuracion de _\_config.yml_ y personalizacion
* Respaldo e implementación de archivos de _GitHub Page_
* Actualización de contenido
* Eliminar, re-crear y modificar _GitHub Page_
* Actualizar contenido y finalizar configuración de la página
* _UP_ de la página

