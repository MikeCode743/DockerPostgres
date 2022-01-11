# Docker Postgres

Este repositorio tiene el objetivo de generar un docker con la ultima version de la imagen de postgres de DockerHub, ademas de incluir un cliente de base de datos PgAdmin4.

El docker esta configurado para ser persistente con la data almacenado, lo que hace posible almacenar y recuperar los datos

### Requisitos

Se debe tener instalado los siguientes programas instalados:

- Git
- Docker

Para iniciar el docker se debe de clonar el repositorio

    https://github.com/MikeCode743/DockerPostgres.git

ejecutar el siguiente comando en la carpeta descargado

    docker-compose up

### Instalara las siguientes imagenes:

- PostgreSQL
- PgAdmin

Postgres estara habilitado en el puerto 5433 en tu maquina local

    puerto: 5433

PgAdmin4 estará habiltado en el puerto 9000 en tu maquina local

    http://localhost:9000

### Parametros

Los parametros de configuracion de postgres seran los siguientes:

    - DATABASE_HOST=127.0.0.1       //Host
    - POSTGRES_USER=postgres        //Usuario
    - POSTGRES_PASSWORD=postgres    //Contraseña
    - POSTGRES_DB=dbtest            //Base de datos

Los parametros de configuracion de PgAdmin son los siguientes:

    PGADMIN_DEFAULT_EMAIL: "admin@desarrollo.com"   //Correo de usuario
    PGADMIN_DEFAULT_PASSWORD: "admin"               //Contraseña

### Informacion

Para mayor informacion revisar los siguientes enlaces

- [docker-compose](https://docs.docker.com/compose/)
- [postgres](https://hub.docker.com/_/postgres)
- [dpage / pgadmin](https://hub.docker.com/r/dpage/pgadmin4)
