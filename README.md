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
