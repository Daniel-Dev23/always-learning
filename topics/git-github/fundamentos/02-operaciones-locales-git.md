# __Operaciones Locales__ 🏆

<img src="https://res.cloudinary.com/daniel-dev23/image/upload/v1664653633/Always%20Learning/GitGithub/operaciones-locales_owm3iy.png" alt="Operaciones Locales" width="600px"/>

<br>

En git, sabemos que existe un __Ciclo de Vida__ que explica de que forma git interactua con los archivos de nuestro proyecto.

Pero existe una mecánica que explica en lineas generales, el procesamiento de los archivos cuando estamos entre la etapa de __Untrack__ y __Stage__. A esto se le conoce como __Operaciones Locales__.

Las operaciones locales, se dividen en tres fases:

1. 👉 __Working Directory:__ Hace referencia al repositorio local, es decir, a los ficheros que vamos a darles seguimiento con Git en nuestro proyecto.

    - En este punto, se suelen aplicar comandos como __"git status"__, __"git add"__ para salir del __Untracked__ y pasar al __Staged__.

2. 👉 __Staging Area:__ Hace referencia al "área de preparación", es decir, el lugar donde tendremos nuestros ficheros listos para ser capturados en el repositorio local.

    - En este punto, se suele aplicar el comando __"git commit"__ para salir del __Staged__ y pasar al estado __Unmodified__.

3. 👉 __Git Directory:__ Hace referencia al repositorio remoto como tal, es decir, donde tenemos el seguimiento y control total de nuestro ficheros.

    - En este punto, los archivos están en un estado __Unmodified__, pues ya se le dieron seguimiento a los ficheros. Si hay nuevos cambios, entonces pasaran al estado __Modified__ y volveremos a la Operación del __Working Directory__ y del __Staging Area__.

---
📌 __[Volver a Git](../index-git-github.md)__