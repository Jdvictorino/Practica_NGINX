# Practica NGINX con Docker

Este proyecto corresponde a la práctica de ejecutar un servidor web Nginx de forma local usando Docker Compose.

## Objetivo

Levantar un contenedor de Nginx que sirva una página HTML estática ubicada en el directorio `src`.

## Estructura del proyecto

- `src/index.html`: página de prueba con el contenido mostrado por Nginx.
- `docker_compose.yml`: configuración del contenedor, puertos y volumen compartido.

## Funcionamiento

1. Se crea el directorio `src` con un archivo `index.html`.
2. El archivo de Docker Compose monta `src` en `/usr/share/nginx/html`.
3. Al ejecutar `docker compose up -d`, Nginx queda disponible en el puerto `80`.
4. Al abrir el navegador en `http://localhost`, se visualiza la página de prueba.

## Verificación

Para comprobar que todo funciona correctamente:

- Iniciar el contenedor con `docker compose up -d`.
- Revisar que el contenedor esté activo.
- Abrir `http://localhost` en el navegador.

## Entrega

La práctica también incluye crear el repositorio Git, subirlo a GitHub y compartir la URL pública en el foro.
