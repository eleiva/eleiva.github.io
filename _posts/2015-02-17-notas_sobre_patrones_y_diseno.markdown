---
title: Maximas de los patrones de diseño
layout: post
category: Development
author: Eduardo Leiva
date: 2015-02-20
---

El objetivo de esta nota es anotar las premisas basicas y fundamentales que todo buen diseño orientado a objetos tiene que tener. Esta nota tendra sentido si tienes el concepto de patrones de diseño pero no lo haz practicado aun. Asi mismo si ya tienes practica no viene mal recordarlos ya que el objetivo sera mejorar nuestro codigo. Algunas recomendaciones que analizaremos son:

* Enfocarse en la responsabilidad de las clases.
* Promover la flexibilidad a travez de la composicion.
* Hacer la jerarquia de la herencia, mas compacta y enfocada.
* Reducir la duplicacion.
* Encapsular el concepto que varia.
* Code to an interface, not to an implementation.


Como veran todos seriamos felices si pudieramos contruir aplicacione que respeten estas ultimas premisas, pero no es una tarea sencilla ya que cada systema ( problema ) tiene un conjunto de caracteristicas diferentes que lo hace nuevo ( nuevo contexto ) y el uso de patrones de diseño nos brindaran algunas soluciones reales a problemas comunes que nos encontramos dia a dia en la construccion de sistemas medianos y grandes.


#### Paternitis 

No siempre necesitamos hacer un diseño complejo ( la idea de diseñar es dar una solucion acertada a un problema en particular )
Si tenemos dudas podemos basarnos en algunos conceptos de XP:

* Do the simplest thing that works
* ou aren’t going to need it” (often abbreviated to YAGNI)

#### Crendo tus objetos

A medida que se hace complejo el sistema, es necearia una buena estrategia para la creacion de los objetos . Para ello tenemos los siguientes patrones:

* The Singleton pattern: Cuando quieres tener un solo objeto de ese tipo en el sistema
* The Factory Method pattern: Tienes que construir objetos complejos? Este es tu patron.
* The Abstract Factory pattern: Tienes que construir objetos complejos distintos?
* The Prototype pattern: En vez de hacer nacer nuestros objetos tipo matrix, los clonamos como la guerra de las galaxias.

Algunas recomendaciones:

Evitar grandes if-switch y llevarlos a la creacion de los objetos.

#### Recordatorio para encontrar un patron

* Because container objects share an interface with the objects that they contain,
they are naturally suited to share a type family.
