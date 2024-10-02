# PHP, APACHE y MYSQL CON DOCKER

### Configuración 
1. Se tiene que instalar docker en su dispositivo, lo más sencillo es descargar [Docker Desktop](https://www.docker.com/products/docker-desktop).
2. Se descargan las imágenes para [PHP](https://hub.docker.com/_/php) y [MySql](https://hub.docker.com/_/mysql):
> Por defecto se descargará la última versión. Si se desea se puede cambiar las versiones de mysql y/o php, si se realiza el cambio de versión, se debe de configurar en Dockerfile y docker-compose.yml
```cli
    docker pull php
```
```cli
    docker pull mysql
```

### Inicialización y Desarrollo
1. Se inicializa el servicio con el comando:
```
    docker compose up -d
```
2. Todos los archivos deben estar dentro de la carpeta: ```app/```.
3. Verificar las credenciales de acceso de la base de datos mysql en ```docker-compose.yml```.
4. Se visualizar en [http://localhost:80](http://localhost:80)