# LAMPP Built by Docker
1. Download & Unzip or Clone the repository
2. Create `data` folder under `mysql`
3. Run `docker-compose` command
    - `$ docker-compose up -d`
4. Open browser and view top pages
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
