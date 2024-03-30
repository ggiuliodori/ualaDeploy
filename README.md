# Guía de Instalación y Uso

Esta guía te ayudará a levantar los servicios necesarios para ejecutar la aplicación utilizando Docker Compose.

## Requisitos Previos

Asegúrate de tener instalado Docker y Docker Compose en tu sistema. Puedes encontrar instrucciones de instalación en la documentación oficial:

- Docker: https://docs.docker.com/get-docker/
- Docker Compose: https://docs.docker.com/compose/install/

## Configuración

El archivo `docker-compose.yml` contiene la configuración para los servicios necesarios. Asegúrate de ajustar cualquier configuración necesaria, como puertos, contraseñas, etc., según sea necesario.

## Pasos para Levantar los Servicios

1. Abre una terminal.
2. Navega al directorio donde se encuentra el archivo `docker-compose.yml`.
3. Ejecuta el siguiente comando para levantar los servicios:

   ```bash
   docker-compose up -d

Este comando levantará todos los servicios en segundo plano (-d).
Espera a que todos los contenedores se inicien correctamente.

## Acceso a los Servicios

Una vez que los servicios estén en funcionamiento, puedes acceder a ellos utilizando los siguientes enlaces:

- Mongo Express: http://localhost:8090
- PHPMyAdmin: http://localhost:8085

Para acceder a los servicios específicos de la aplicación, puedes utilizar las siguientes direcciones:

- User Service: http://localhost:8081
- Tweet Service: http://localhost:8082
- Timeline Service: http://localhost:8083

## Detener los Servicios

Para detener los servicios, ejecuta el siguiente comando en la misma terminal donde levantaste los servicios:

 ```bash
   docker-compose down
