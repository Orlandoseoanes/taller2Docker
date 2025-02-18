# FastAPI App con Docker

Este proyecto es un ejemplo práctico de cómo crear y desplegar una aplicación FastAPI utilizando Docker. A continuación, se describen los pasos para construir la imagen Docker, ejecutar el contenedor y subir la imagen a Docker Hub.

## Requisitos

- [Docker](https://www.docker.com/get-started) instalado en tu máquina.
- (Opcional) Cuenta en [Docker Hub](https://hub.docker.com/).
- Conocimientos básicos de Python y FastAPI.

## Estructura del Proyecto

- **Dockerfile:** Instrucciones para construir la imagen Docker.
- **requirements.txt:** Lista de dependencias, que debe incluir FastAPI y Uvicorn.
- **app/main.py:** Código fuente de la aplicación FastAPI.

## Construcción de la Imagen Docker

Para construir la imagen, navega al directorio del proyecto y ejecuta:

```sh
docker build -t oaseoanes/fastapi-app:latest .


docker run -d -p 8000:80 --name fastapi-container oaseoanes/fastapi-app
