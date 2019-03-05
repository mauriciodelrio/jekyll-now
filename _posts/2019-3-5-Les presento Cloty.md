---
layout: post
title: Les Presento Cloty
---

Hace mucho tiempo que no creaba una entrada en mi blog y lo tengo realmente pendiente, hace unos meses estuve trabajando de forma colaborativa con compañeros de universidad, y a uno de ellos se le ocurrió la idea de crear una aplicación pensada para recomendar ropa según tus gustos, el clima, tus elecciones anteriores y el gusto colectivo.

Así es como nace Cloty.

![]({{ site.baseurl }}/images/cloty/2.png)

### ¿Qué es exactamente Cloty?

Cloty es un proyecto experimental que permite registrar tu ropa creando un "Ropero", el cual te ofrece una cantidad de ropa según la categorización disponible en el sistema. Al registrar tu ropa, tienes la posibilidad de registrar una foto de ella.

Cloty es una aplicación Mobile que funciona en segundo plano, es decir, la lógica del producto final es que como usuario final programes una hora prudente en donde cloty te dirá la temperatura de hoy en tu ciudad y te dará un set de recomendaciones de outfit. Esto será notificado a tu celular a través de una notificación push. Puedes aceptar uno y rechar el resto. La idea original es que mediante el feedback que entrega el usuario informando al sistema si usó el atuendo o no, vaya alimentando una red neuronal la cual aprenderá de tus gustos y perfeccionará las elecciones futuras.

Como proyecto experimental, la idea es sencilla, integrar en un sistema relativamente simple conceptos complejos que permiten transformar un concepto simple en algo que pueda volverse vanguardista.

### Algunas características iniciales

* Registro de usuarios
* Registrar ropa según categorías permitiendo asignar una foto por cada prenda
* Crear un sistema externo que recoja datos de clima según geolocalización
* Solicitar recomendación de forma manual al sistema de combinaciones de prendas que posean un sentido lógico.
* Generar un servicio de entrenamiento generando una red neuronal que se retroalimente con los parámetros ya mencionados.
* Permitir al usuario entregar feedback sobre que atuendo desea elegir en un día en particular.

![]({{ site.baseurl }}/images/cloty/1.png "Acá algún ejemplo visual")


Por decisión de equipo, Cloty no es un trabajo de código abierto, uno de nuestros integrantes del equipo desea seguir con el proyecto, por ende, respetamos la autoría, sin embargo mostraré por acá algunas capturas de como se ve el producto en una primera fase.


### Arquitectura

En este punto debo detenerme, la arquitectura de este proyecto se basa en servicios que viven de forma independiente pero que se comunican entre ellos a través de métodos en específico. Pueden ver un diagrama explicativo del modelo conceptual a continuación.

![]({{ site.baseurl }}/images/cloty/3.png)


Como se observa, el modelo muestra un servicio de climatología, un servicio de backend y un servicio de entrenamiento. Cada uno de ellos trabaja con diversos stacks tecnológicos, a continuación les presento el stack de cada uno de ellos.

![]({{ site.baseurl }}/images/cloty/4.png)

![]({{ site.baseurl }}/images/cloty/5.png)

![]({{ site.baseurl }}/images/cloty/6.png)

![]({{ site.baseurl }}/images/cloty/7.png)


Es importante señalar que esto es un *prototipo de aplicación*, no está finalizado, sin embargo, hay altas expectativas con este proyecto. En particular mi labor acá fue trabajar y construir el servicio de climatología y el backend de la aplicación. Pude revisar y entender la forma en que opera la red neuronal, eso lo es un tema un poco más largo y lo podemos dejar para otra entrada de blog.

### Contáctame

Si estás interesado en participar, me puedes escribir a [Mi mail](mailto:mauricio.delr@gmail.com).
Yo te puedo poner en contacto con la persona que sigue con este proyecto.

Saludos y nos vemos en otra entrada! 
