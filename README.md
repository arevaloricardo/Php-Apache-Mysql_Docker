# PHP, APACHE y MYSQL CON DOCKER

### 1. Configuración 
1.1. Se tiene que instalar docker en su dispositivo, lo más sencillo es descargar [Docker Desktop](https://www.docker.com/products/docker-desktop).  
1.2. (Opcional) Se descargan las imágenes para [PHP](https://hub.docker.com/_/php) y [MySql](https://hub.docker.com/_/mysql) 
```cli
docker pull php
```
```cli
docker pull mysql
```
> Se puede omitir este paso debido a que cuando se inicializa como lo especifica el punto 2.1 se descarga automaticamente las imagenes correspondientes.  
  
> Por defecto se descargará la última versión. Si se desea se puede cambiar las versiones de mysql y/o php, se debe de configurar en Dockerfile y docker-compose.yml

### 2. Inicialización y Desarrollo
2.1. Se inicializa el servicio con el comando:
```
docker compose up -d
```
2.2. Todos los archivos deben estar dentro de la carpeta: ```app/```.  
2.3 Verificar las credenciales de acceso de la base de datos mysql en ```docker-compose.yml```.  
2.4 Se puede visualizar en localhost:80