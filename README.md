# -S4-Crear-tu-Primera-Base-de-Datos-en-PostgreSQL-usando-Docker-y-DataGrip

##  Descripción

En esta actividad se realizó la instalación y configuración de PostgreSQL utilizando Docker como entorno de ejecución, y DataGrip como IDE para administrar y trabajar con la base de datos.

El objetivo principal es levantar un servidor PostgreSQL dentro de un contenedor Docker, establecer una conexión desde DataGrip y crear una primera base de datos llamada `my_first_database`.

---

##  Objetivos

- Instalar y verificar Docker Desktop.
- Ejecutar PostgreSQL mediante un contenedor Docker.
- Verificar que el contenedor de PostgreSQL se encuentre activo.
- Instalar y configurar DataGrip.
- Conectar DataGrip con PostgreSQL.
- Crear una nueva base de datos desde una consola SQL de DataGrip.
- Documentar el procedimiento realizado.

---

#  1. Instalación de Docker

Para ejecutar PostgreSQL mediante Docker es necesario tener Docker Desktop instalado.

Docker Desktop permite crear y administrar contenedores desde Windows y proporciona las herramientas necesarias para ejecutar PostgreSQL de manera aislada.

### Descarga

Docker Desktop puede descargarse desde:

https://www.docker.com/products/docker-desktop/

Después de instalar Docker Desktop, se debe iniciar la aplicación y verificar que Docker esté funcionando correctamente.

### Verificación

Desde una terminal se puede comprobar que Docker está instalado correctamente ejecutando:

```bash
docker --version

Descargar e iniciar PostgreSQL en Docker

Con Docker Desktop instalado y funcionando, se abre una terminal y se ejecuta el siguiente comando para descargar e iniciar PostgreSQL mediante Docker:

docker run --name postgres-db -e POSTGRES_PASSWORD=yourpassword -p 5432:5432 -d postgres

Este comando crea un contenedor llamado postgres-db, establece yourpassword como contraseña del usuario postgres, conecta el puerto 5432 del contenedor con el puerto 5432 del equipo y ejecuta PostgreSQL en segundo plano.

Para comprobar que el contenedor de PostgreSQL se encuentra activo se ejecuta:

docker ps

El contenedor postgres-db debe aparecer en la lista de contenedores activos.

Instalación de DataGrip

Una vez iniciado PostgreSQL en Docker, se debe descargar e instalar DataGrip desde:

https://www.jetbrains.com/datagrip/download

Después de instalar DataGrip, se debe abrir el programa y registrar la licencia gratuita utilizando el correo institucional de la UMG.

Configuración en DataGrip

Para configurar la conexión con PostgreSQL en DataGrip se debe ingresar a:

File > Data Sources and Drivers

Luego se debe hacer clic en + y seleccionar PostgreSQL.

Se configuran los siguientes datos:

Host: localhost
Port: 5432
User: postgres
Password: yourpassword
Database: postgres

Después de ingresar los datos, se debe realizar una prueba de conexión para verificar que DataGrip pueda conectarse correctamente con PostgreSQL.

Crear tu Base de Datos

Una vez establecida la conexión con PostgreSQL, se debe abrir una nueva consola SQL en DataGrip.

En la consola se ejecuta:

CREATE DATABASE my_first_database WITH TEMPLATE template0;

Este comando crea una nueva base de datos llamada my_first_database utilizando template0 como plantilla.

Después de ejecutar el comando, se debe verificar en DataGrip que la base de datos my_first_database haya sido creada correctamente.

