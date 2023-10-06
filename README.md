# LAMPP Built by Docker
1. Download and Install [Docker Desktop](https://www.docker.com/products/docker-desktop/)
2. Download & Unzip or Clone the repository
3. Create `data` folder under `mysql`
4. Run `docker-compose` command
    - `$ docker-compose up -d`
5. Open browser and view top pages
    - `http://localhost` (web home)
    - `http://localhost:8080` (phpmyadmin)
   
# Usefull Docker Commands
1. start docker
    - `$ docker-compose up -d`
    - `$ docker compose up -d`
2. list containers
    - `$ docker ps`
3. enter the shell of a container
    - `$ docker exec -it <container-name> /bin/bash`
4. build an image from Dockerfile
    - `$ docker build [<path>|<utl>|-]`
5. download an image from a registry
    - `$ docker pull <url>`
6. list images
    - `$ docker images`
