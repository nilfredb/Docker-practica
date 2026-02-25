Descripción del Proyecto

Este proyecto demuestra cómo desplegar un servidor web Nginx en local
utilizando Docker Compose. El servidor muestra una página HTML sencilla
(“Hola Mundo”) desde un directorio local montado como volumen dentro del
contenedor.

Tecnologías Utilizadas

-   Docker
-   Docker Compose
-   Nginx

Estructura del Proyecto

nginx-docker-practica/ │ ├── docker-compose.yml └── src/ └── index.html

Instrucciones de Uso

1.  Clonar el repositorio: `git clone https://github.com/nilfredb/Docker-practica.git`

2.  cd nginx-docker-practica

3.  Iniciar el contenedor: docker compose up -d

4.  Abrir el navegador y visitar: http://localhost:8080

Cómo Funciona

-   El contenedor Nginx expone internamente el puerto 80.
-   El puerto 8080 del host está mapeado al puerto 80 del contenedor.
-   El directorio local ./src se monta en /usr/share/nginx/html dentro
    del contenedor.
-   Cualquier cambio realizado en index.html se refleja automáticamente
    en el navegador gracias al uso de volúmenes.

Detener el Servidor

Para detener el contenedor en ejecución: docker compose down

Autor

Nilfred Baez