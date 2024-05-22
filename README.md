# Mi-primer-servidor-HTTP

#2) Servidor simple de hola mundo en Node.js usando HTTP:

    El código crea un servidor HTTP simple que escucha en el puerto 4444.
    Cuando se hace una solicitud al servidor, responde con un archivo específico si la URL coincide con ciertas rutas (por ejemplo, / sirve el archivo index.html).
    Si no se encuentra el archivo solicitado, responde con un mensaje de "Not found".

#3) Servidor síncrono que lea y envíe un archivo:

    El código utiliza la función fs.readFile para leer archivos de forma asíncrona.
    Cuando se recibe una solicitud, intenta leer el archivo correspondiente de manera asíncrona y luego envía su contenido como respuesta.

#4) Servidor asíncrono que lea y envíe un archivo:

    El código utiliza la función fs.readFile para leer archivos de forma asíncrona, como en el punto anterior.
    Sin embargo, este servidor también tiene una ruta especial /registro que maneja datos enviados mediante una solicitud POST. Cuando se recibe una solicitud en esta ruta, los datos se leen de manera asíncrona y se envían como respuesta.

#5) Servidor asíncrono que lea y envíe un archivo según su extensión:

    Este es similar al punto 4, pero con la adición de un switch que determina el tipo MIME de la respuesta según la extensión del archivo solicitado.
    Dependiendo de la extensión del archivo solicitado, el servidor responde con el tipo MIME correspondiente (text/plain, text/html, image/jpg, etc.).
