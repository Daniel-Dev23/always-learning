# __Teoría de Uniones__ 🏆

<img src="https://res.cloudinary.com/daniel-dev23/image/upload/v1664653633/Always%20Learning/GitGithub/merge-branch_qyje4v.png" alt="Merge Branch" width="400px"/>

<br>

La teoría de uniones o mejor conocido como __Merge-Branch__ es uno de los más importantes, porque en git tenemos el cocepto de __Branch o "ramas"__. 

Las __ramas__ (branch), son entornos o ramificaciones que se construyen a partir de una __rama principal__ para trabajar código en ese entorno. Cuando se crean ramas, estos generan exactamente el mismo contenido que la rama principal.

Esto es una ventaja, porque de esta manera, no estamos obligados a trabajar sobre la rama principal. Si comentemos errores y no tenemos cierta organización, todo el control de nuestro código con git, puede ser caotico.

En su lugar, podemos crear otra rama para hacer y deshacer ahí, antes de crear una versión ideal del proyecto.

Luego de conocer las ramas, __¿Qué tiene que ver el merge?__

## __Tipos de Git Merge__

Un __merge__ es sencillamente la unión de ramas. Así como podemos crear "copias" de otras ramas, también podemos unirlas entre si para crear un solo contenido o entorno.

Esta es una práctica a la que vamos a estar expuestos casi siempre. Sin embargo, tienes que saber que existen 3 tipos de merge:

- 👉 __Fast Forward:__  Hace referencia a que git pudo
identificar todos los nuevos cambios entre la __"rama A"__ y la __"rama B"__ sin problema y al unirlos, no hubo ningún conflicto. Este es el mejor de los casos.
- 👉 __Unión Automática:__ La unión automática en git, se genera solo si se cumplen las siguientes condiciones:

    - Cuando en la __"rama A"__ hay cambios, pero aún no se han agregado los cambios de la __"rama B"__.

    - Cuando en la __"rama B"__ hay cambios, pero estos aún no se han unido con la __"rama A"__.

    - Si no hay conflictos. En otras palabras, si en la __"rama A"__ y __"rama B"__, no se han modificado los mismos archivos.

    Si se cumplen esas condiciones, al momento de hacer la unión, git solicitará que se realice un nuevo commit para unir todas las ramas de B hacia la rama A, que sería la principal.

- 👉 __Unión con Conflictos:__ Esto sucede, cuando se han aplicado cambios en el mismo archivo en la __"rama A"__ y en la __"rama B"__ o incluso en las mismas líneas de código.

    Git, notará que los cambios en __"rama A"__ y __"rama B"__ no coinciden, por lo tanto, no podrá hacer mucho ante eso. En su lugar, __git cede el control al usuario para que decida, que quiere conservar o eliminar__.
    
    El usuario, toma la decisión y entonces para terminar el conflicto, solo necesita aplicar un __git add__ y un __git commit__.

    🌟 __Durante este tipo de merge, los archivos que no tengan conflicto, pasaran sin problema.__

---
📌 __[Volver a Git](../index-git-github.md)__