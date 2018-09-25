---
layout: post
title: Les presento Carbon
---

Hoy les traigo otro proyecto educativo, como estudiantes o ex estudiantes sabrán que una de las cosas más engorrosas en los establecimientos educacionales es el poder compartirse material de estudios entre alumnos de generación, de diversos cursos, con mayor razón, es complejo también el compartir material con estudiantes que cursan asignaturas similares pero en otras instituciones, no existiendo a la fecha, ningún medio formal en donde se puede acceder libremente al material liberado, de uso público para la socialización del conocimiento. Bajo esta premisa nace Carbon.

![]({{ site.baseurl }}/images/carbon/horizontal.png)

### ¿Por qué Carbon?

Carbon nace bajo el concepto de red social educativa, la idea en sí es vincular universidades para que los estudiantes puedan compartir sus aportes, recibir valoraciones y opiniones por éstos, así, generar retroalimentación entre la comunidad, destacando los grandes aportes que se pueden realizar. Por otra parte las instituciones pueden reguar el contenido asociado a ellas y monitorear que no exista violación a la propiedad intelectual.

### Algunas características iniciales

* Roles de usuario y tipos de pefiles asociados
* Posibilidad de gestionar usuarios y material subido *pendiente la posibilidad de administración absoluta del sistema*
* Caja de comentarios de facebook
* Búsqueda y filtros inteligentes de material para facilitar al estudiante la obtención del mismo.
* Integración con google drive *A evaluar el hecho de contener los archivos de otra forma*

![]({{ site.baseurl }}/images/carbon/c1.png "Acá algún ejemplo visual")


Carbon es código abierto, sin fines de lucro, dejo el link al repositorio acá: 

####  [Carbon-back](https://github.com/mauriciodelrio/carbon)   [Carbon-front](https://github.com/mauriciodelrio/carbon-front)

La idea es que lo puedan visitar, y contribuir en el desarrollo de un producto pensado para comunidades educativas organizadas.

Acá les dejo un aproach del modelo de datos que utiliza en cuestión:

![]({{ site.baseurl }}/images/carbon/MAnalisiscompletofinal.png)


###  Tecnologías

* Redis para el manejo de concurrencia.
* Postgresql (10.XX) para el contenedor de datos
* Node (8.xx) + Express Para el manejo de servidor y peticiones HTTP.
* React-Redux para client side.
* El servicio vive en dos máquinas distintas.

Es importante señalar que esto es un *prototipo de aplicación*, no está finalizado, sin embargo, a futuro me gustaría concretarlo.

### Contáctame

Si estás interesado en participar, me puedes escribir a [Mi mail](mailto:mauricio.delr@gmail.com).
Estaré feliz de tener amigos con quién colaborar.

Saludos! 
