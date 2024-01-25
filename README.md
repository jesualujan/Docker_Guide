# 🌐 Redes Sociales: [![Facebook](https://img.shields.io/badge/Facebook-%231877F2.svg?logo=Facebook&logoColor=white)](https://www.facebook.com/profile.php?id=100093507976508&mibextid=gik2fB) [![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jesua-hadai-alderete-luj%C3%A1n-a2325a121/) 
<p>Elaborado por: Jesua Luján</p> 

<h1> Aprendiendo Docker 👨‍🎓 </h1> 
 <h2> 🐳 Docker empaqueta software en unidades estandarizadas llamadas contenedores que incluyen todo lo necesario para que el software se ejecute, incluidas bibliotecas, sistemas operativos, código, testing, bases de datos y tiempo de ejecución.
La idea detrás de Docker es crear contenedores ligeros y portables para las aplicaciones de software que puedan ejecutarse en cualquier máquina con Docker instalado, independientemente del sistema operativo que la máquina tenga por debajo,
 facilitando así también los despliegues. </h2>


  ![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white) # SE COMPONE EN 3 PARTES PRINCIPALES:

    1) DOCKER FILES
    2) DOCKER IMAGES
    3) DOCKER CONTAINERS
    
![image](https://github.com/jesualujan/Docker_Guide/assets/56859580/6a73e86b-c4a0-4280-a1e2-f0faf91aad44)
 
<H3>Como Instalar docker:</H3>
<table>
        <thead>
            <tr>
                <th>SISTEMA OPERATIVO</th>
                <th>SIGNFICADO</th>
                <th>SINTAXIS</th>
            </tr>
        <tbody>
            <tr>
                <td>Para Windows</td>
                <td><p>este comando te ayudará a instalar docker en Windows</p></td>
                <td><p>https://download.docker.com/win/stable/InstallDocker.msi</p></td>
            <tr>
                <td>Para Linux</td>
                <td><p>este comando te ayudará a instalar docker en Linux</p></td>
                <td><p>curl -sSL https://get.docker.com/ | sh</p></td>
            <tr>
                <td>Para Mac</td>
                <td><p>este comando te ayudará a instalar docker en Mac</p></td>
                <td><p>https://download.docker.com/mac/stable/Docker.dmg</p></td>
        </tbody>
    </table>

 <p> 2. Registro de Docker y Repositorio  </p>
    <table>
        <thead>
            <tr>
                <th>Comando</th>
                <th>SIGNFICADO</th>
                <th>SINTAXIS</th>
            </tr>
        <tbody>
            <tr>
                <td>Login to a Registry</td>
                <td><p>This command helps you log in to your Registry.</p></td>
                <td><p>docker login
                    docker login localhost:8080</p></td>
            <tr>
                <td>Logout from a registry:</td>
                <td><p>This command helps you log out from your Registry.</p></td>
                <td><p>docker logout
                    docker logout localhost:8080</p></td>
            <tr>
                <td>Searching an image</td>
                <td><p>By using this docker command you can search any image from your docker.</p></td>
                <td><p>search nginx
                    docker search --filter stars=3 --no-trunc nginx</p></td>
                    <tr>
                        <td>Pulling an Image</td>
                        <td><p>This command can be used to download a specific image or set of images.</p></td>
                        <td><p>docker image pull nginx
                            docker image pull eon01/nginx localhost:5000/myadmin/nginx</p></td>
                            <tr>
                                <td>Pushing an image</td>
                                <td><p>This command can be used to push a specific image or set of images.</p></td>
                                <td><p>docker image push eon01/nginx
                                    docker image push eon01/nginx localhost:5000/myadmin/nginx</p></td>
        </tbody>
    </table>
    <p> 4. comandos para arrancar/iniciar o detener un contenedor </p>
    <table>
        <thead>
            <tr>
                <th>COMANDO</th>
                <th>SIGNFICADO</th>
                <th>SINTAXIS</th>
            </tr>
        <tbody>
            <tr>
                <td>Command for starting a container</td>
                <td>
                    <p>This command is used for starting a container </p>
                </td>
                <td>
                    <p>docker container start nginx</p>
                </td>
            <tr>
                <td>Command for stopping a container</td>
                <td>
                    <p>This command is used for stopping a container</p>
                </td>
                <td>
                    <p>docker container stop nginx</p>
                </td>
            <tr>
                <td>Command for restarting the container</td>
                <td>
                    <p>This command is used for restarting a container</p>
                </td>
                <td>
                    <p>docker container restart nginx</p>
                </td>
            <tr>
                <td>Command for pausing the container</td>
                <td>
                    <p>This command is used for pausing a container</p>
                </td>
                <td>
                    <p>docker container pause nginx</p>
                </td>
            <tr>
                <td>Command for unpausing the container</td>
                <td>
                    <p>This command is used for unpausing a container in the docker </p>
                </td>
                <td>
                    <p>docker container unpause nginx</p>
                </td>
                <tr>
                    <td>Command for Blocking a container</td>
                    <td>
                        <p>This command is used for blocking a container in the docker  </p>
                    </td>
                    <td>
                        <p>docker container wait nginx</p>
                    </td>
                    <tr>
                        <td>Sending a SIGKILL</td>
                        <td>
                            <p>This command is used for Sending a SIGKILL in the docker </p>
                        </td>
                        <td>
                            <p>docker container kill nginx</p>
                        </td>
                        <tr>
                            <td>Command for sending another signal</td>
                            <td>
                                <p>This command is used for for sending another signal</p>
                            </td>
                            <td>
                                <p>docker container kill -s HUP nginx</p>
                            </td>
                            <tr>
                                <td>Command for Connecting to an Existing Container</td>
                                <td>
                                    <p>We can use this command for Command for Connecting to an Existing Container</p>
                                </td>
                                <td>
                                    <p>docker container attach nginx</p>
                                </td>
        </tbody>
    </table>

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

