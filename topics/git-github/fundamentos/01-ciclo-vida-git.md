# __Ciclo de Vida de Archivos en Git__ 🏆

El ciclo de vida en git, es uno de los flujos más importantes para estudiar y comprender. Hace referencia al estado de los archivos cuando estan siendo analizados por el algoritmo de git en el repositorio local.

<img src="https://res.cloudinary.com/daniel-dev23/image/upload/v1664653633/Always%20Learning/GitGithub/ciclo-vida-git_eopd2m.png" alt="Ciclo de Vida en Github" width="600px"/>

<br>

El ciclo de vida consiste en las siguientes etapas:

- 👉 __Untracked (Sin seguimiento):__ Hace referencia a los archivos que aún no tienen seguimiento de parte de git.

- 👉 __Unmodified (Sin modificación):__ Indica que los archivos a los que git les esta dando seguimiento, no tienen modificaciones para capturar. 

- 👉 __Modified (Modificación):__ Indica que los archivos a los que git les esta dando seguimiento, han tenido modificaciones. A su vez este es un aviso de que los nuevos cambios necesitan ser capturados.

- 👉 __Staged (Preparado):__ Hace referencia, a que los archivos estan preparados para ser capturados en el __Git Directory__.

## __Explicación__

1. ✅ Por defecto, los archivos comienzan por no tener seguimiento en git, en este punto se dice que los archivos están en etapa __untracked__ o sin seguimiento. 

    Es ahí cuando debemos aplicar comandos como __"git status"__, __"git add ."__ para poder preparar __(Staged)__ los archivos y capturarlos en el repositorio local.

2. ✅ Una vez que los archivos estan preparados __(Staged)__, entonces se realiza un __"git commit"__ para colocarlo en el __Git Directory__. 

    Después de que se aplica el commit, los archivos pasan a tener el estado __Unmodified (Sin modificación)__, esto quiere decir, que no hay modificaciones en los archivos del proyecto. Esto es lógico, pues en teoría, ya estamos dando seguimiento al código.

3. ✅ Pero, cuando seguimos avanzando con nuestro proyecto y hacemos modificaciones, git es tan inteligente, que es capaz de identificar que hay nuevos cambios que necesitan estár capturados. 

    Es ahí donde los archivos pasan a tener el estado de __Modified (Modificación)__. Para salir de este estado, tenemos que volver a aplicar comandos como __"git status"__, __"git add ."__ para preparar __(Staged)__ los archivos y después hacer __git commit__ volver al estado de __Untrack__.

---
📌 __[Volver a Git](../index-git-github.md)__