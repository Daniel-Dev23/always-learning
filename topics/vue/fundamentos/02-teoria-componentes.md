# __Teoría de Componentes__ 🏆

La mayoría de frameworks o librerias basadas en Javascript moderno, trabajan a base de __componentes__, por lo que este tema es elemental.

__¿Y cuál es la razón?__ Los creadores de Vue, notaron que en el desarrollo frontend de años atrás, la mayoría de aplicaciones llegaban a un punto donde se enfrentaban al consumo masivo de información. 

Cuando esto sucedía, eso era un indicío fuerte de que los desarrolladores se verían en la necesidad de crear muchas vistas o interfaces de usuario.

Esto a nivel estructural era un problema. No existian muchas alternativas que ofrecieran eficiencia a la hora de crear e implementar vistas y los que existian, eran bastante rudimentarios, por lo que el beneficio no era tan marcado.

Fue así que llega Vue JS con una propuesta innovadora, trabajando con componentes, los cuales te permiten __modularizar la lógica de negocio__ en diferentes vistas, haciendolas reutilizables.

Los __componentes__ concisten en una mecánica la cual, dependiendo del estado de nuestra información, es lo que se va a renderizar hacia el usuario (aquí se implementa la reactividad).

Esta, fue la eficacia que muchos desarrolladores frontend buscaban: __algo que fuera intuitivo, reutilizable y fácil de implementar.__

Para que un módulo pueda ser considerado un componente, debe cumplir con las siguietes características:

- __Son un fragmento__ de la interfaz que cumplen una función única.

- __Son reutlizables__, aplicando el principio DRY (Don't Repeat Yourself).

- __Son independientes__, tanto de su contexto como del resto de componentes. Puedes retutilizar es componente en otro ambito y debería seguir funcionando igual.

- __Son autocontenidos__, eso quiere decir, que no filtran estilos, ni lógica de otro negocio a otro componentes.

---
📌 __[Volver a Vue JS Topics](../index-vue.md)__