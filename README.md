
# INTRODUCCIÓN A DOCKER 

DOCKER SE COMPONE EN 3 PARTES PRINCIPALES:

    1) DOCKER FILES
    2) DOCKER IMAGES
    3) DOCKER CONTAINERS


La idea de docker es como trabajar una maquina virtual y si, es parecido a una maquina virtual, pero no lo es, la idea es tener un espacio de trabajo, configurado con tecnologías que se desean ocupar en un contenedor, como pueden ser React, Vite, Angular, Express, GraphQL,MongoDB, Etc...

# PRIMEROS PASOS
 * Primero debemos descargar e instalar docker en nuestros sistemas operativos, si estamos en windows debemos actualizar nuestra versión de WSL (subsistemas de linux para windows)

* Para realizar la descarga de docker debemos ir al siguiente enlace:
    https://www.docker.com/get-started/ 
## COMANDOS POSTGRES
Para este ejemplo vamos a utilizar postgres, para ello vamos al sitio de dockerhub:
    https://hub.docker.com/_/postgres

ahí nos sugiere hacer: __docker pull postgres__
pero no es necesario, podemos hacer direcatamente lo siguiente:

    docker run postgres

y con esto se nos bajara la imagen de postgres 

después nos dara el siguiente error en consola: 

      Error: Database is uninitialized and superuser password is not specified.
      You must specify POSTGRES_PASSWORD to a non-empty value for the
     superuser. For example, "-e POSTGRES_PASSWORD=password" on "docker run".

para resolverlo escribimos lo siguiente en la consola:

* docker run -e POSTGRES_PASSWORD=password postgres

y como podemos observar en la terminal ya está corriendo postgres.
Esto pasa porque en la documentación de postgres nos pide una variable de entorno lo cual recibe como parametro una contraseña =)

## COMANDOS UBUNTU

En otra terminal vamos a hacer docker pull de ubuntu hacemos el mismo proceso la podemos buscar en:
    https://hub.docker.com/_/ubuntu

    docker pull ubuntu

## COMANDOS BÁSICOS DE DOCKER

    docker images -> muestra una lista de las images.
    docker ps -> muestra info de los contenedores en ejecución
    docker ps -a -> muestra todos los contenedores.
    docker logs id , docker logs name_container -> se utiliza para ver los registros (logs) de un contenedor específico.
    docker exec -> se utiliza para ejecutar comandos dentro de un contenedor en ejecución. 
    docker exec -it id sh -> muestra información del contenedor
    para salir podemos escribir: exit  
    o bien presionar CTRL + D
    docker stop id -> detiene la ejecución de un contenedor
## Authors

- [jesua luján](https://github.com/jesualujan/jesualujan)

