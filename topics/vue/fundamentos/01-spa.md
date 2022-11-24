# __SPA__ 🏆

SPA, es un concepto que proviene de las siglas:

- __S__ ingle
- __P__ age
- __A__ pplication

O en español, __Aplicaciones de Una Sola Página__.

Las __Single Page Application__, son aplicaciones donde la renderización de contenido, ocurre en un solo lugar del sitio.

Para entender mejor este concepto, a continuación explicaré como funciona la nevagación tradicional, solo para tenerlo como referencia.

## ✅ __Navegación Web Tradicional__

A continuación describo el flujo de una navegación web tradicional:

- 👉 Cuando un usuario ingresa a un sitio web, internamente el sitio web o el __cliente__, hace una solicitud de recursos al __servidor__.

- 👉 El __servidor__, tiene que retornar algo al __cliente__, sin embargo, en este paso el __servidor__ suele tener algunas consideraciones:

    - 📌 Si el recurso __existe__, pueden ocurrir dos escenarios:
    
        - 🤷‍♂️ El recurso __existe y no hay errores__ en el proceso, por lo tanto, el servidor retornará un documento __HTML__, un __JSON__, un __CSV__ o cualquier otro recurso con origen especifíco.

        - 🤷‍♂️ El recurso __existe, pero ocurre un error crítico o inesperado__, por lo tanto, el servidor retornorá un __Error 500__, indicativo de un __Error Interno de Servidor__.

    - 📌 Si el recurso __no existe__, entonces el servidor retornará un __Error 404__, indicativo de una __Página No Encontrada__.

- 👉 En ocasiones, el sitio o aplicativo podría tener interacción de otro origen:

    - Inicio de Sesión.
    - CRUD de un recurso (Create, Read, Update, Delete).
    - Autenticaciones.
    - Autorizaciones.

- 👉 Sea cual sea la interacción, el flujo sigue siendo el mismo: donde el __cliente solicita__ y el __servidor responde__.

- 👉 Cuando el __servidor__ retorna un recurso y el __cliente__ lo recibe, este actualiza y renderiza todo el sitio completamente. Y este proceso se repite ciclicamente.

A esta navegación web tradicional, se le conoce como __Arquitectura Cliente-Servidor__.


## ✅ __Navegación Web SPA__

Teniendo en cuenta la explicación anterior, donde se maneja una __Arquitectura Cliente-Servidor__, como navegación web tradicional, ¿Qué tiene de especial la navegación web en una SPA?

Dentro de un mecánismo SPA: 

- 👉 El __cliente__ hace una solicitud de recursos al __servidor__.

- 👉 El __servidor__ retorna "x" recurso (O bien puede retornar un error).

- 👉 Cuando el __cliente__ hace una nueva solicitud al __servidor__, el recurso se renderiza __SOBRE EL LUGAR__ del recurso que estaba anteriormente.

- 👉 Esto hace que el recurso o contenido que estaba en un inicio, sea "vaciado" o "limpiado" por el __cliente__ y en su lugar renderice el nuevo recurso o contenido.

- 👉 Al aplicarse de este modo, ya no ocurre la actualización de todo el sitio por completo, sino que únicamente se actualiza, lo que se necesita o haga falta, interesante, ¿Cierto?

## ✅ __Ventajas y Desventajas de SPA__

👉 __Ventajas:__

- Tras la carga inicial, da el efecto de una experiencia fluida y rápida.

- Menor estrés para el servidor.

- El caché puede reducir peticiones.

- Mejor experiencia de usuario.

- Carga independiente de módulos cuando son necesarios (aplicación de Lazy Loading).

👉 __Desventajas:__

- No es bueno para implementar SEO (Search Engine Optimization).

- Un cambio pequeño puede requerir un build completo.

- La carga inicial puede llegar a ser pesada (depende mucho de su implementación).

---
📌 __[Volver a Vue JS Topics](../index-vue.md)__