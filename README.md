# integrador-deployment
Facilita el despliegue de cada uno de los contenedores que conforman la aplicación. Este archivo debe estar en la misma carpeta en la que se clonan el resto de repositorios de la aplicación.

Se debe instalar previamente [`docker-compose`](https://docs.docker.com/compose/install/) en el servidor que se desee desplegar la aplicación.

## Instrucciones
Clonar este repositorio
```console
  $ git clone https://github.com/integrador-jsd/integrador-deployment.git
```
Dentro de él, clonar los repositorios que componen la aplicación
```console
  cd integrador-deployment/
  git clone https://github.com/integrador-jsd/integrador-backend.git
  git clone https://github.com/integrador-jsd/integrador-database.git
```

Para crear los contenedores:

```console
  docker-compose build
```

Para iniciar los contenedores:

```console
  docker-compose up -d
```
