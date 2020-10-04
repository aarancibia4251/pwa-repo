# Ciclos de vida del Service

**Descarga**<br>
    Cuando realizas una llamada a .register de cliente(página), se descarga el primer serviceWorker, si la promea fue exitosa comienza el siguiente paso de Instalación sino se rechaza la promesa de registro y se descarta el serviceWorker.
    <hr>
**Instalación**<br>
    Es el primero que obtiene un service Worker y solo sucede una vez, es aqui donde se va a interactuar con la API CACHE para poder guardar los archivos estáticos.
    <hr>
**Activación**
<br>
    En este evento el serviceWorker ya comienza a tener el control total de la aplicación y listo para escuchar toda acción entre la aplicación y la red. Por lo general aqui se actualiza la cache (eliminando la anterior y agregando la nueva que llega en el serviceWorker).

Sigamos con [API CACHE Y API INDEXEDDB](./api-cache-indexed.md)