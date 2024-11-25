# LAMPP on Docker
1. Download and Install [Docker Desktop](https://www.docker.com/products/docker-desktop/)
2. Download & Unzip or Clone the repository, in folder such as `c:\dev\lampp-docker8`
    - `$ cd c:\dev\lampp-docker8`
4. Run `docker-compose` command
    - `$ docker-compose up -d`
5. Open browser and view top pages
    - `http://localhost` (web home)
    - `http://localhost:8080` (phpmyadmin)

# How to Connect to MySQL in PHP
- `$conn = new mysqli("mysql",<user>,<passwd>, <db_name>);`
    - database user accounts (userid/passwd): `root`/`root`, `test`/`test`     

# Useful Docker Commands
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

# Install Docker 
## Install on Linux Machine
1. Enable `centos-extras`
```
$ sudo yum install epel-release
```
2. Setup Repository

```
$ sudo yum install -y yum-utils \
  device-mapper-persistent-data \
  lvm2
```
3. Install Docker Engine

```
$ sudo yum install docker-ce 
```

## Install on Windows Machine
1. Enable Virtualization at BIOS
2. Install/Update `wsl2`
```
$ wsl --update
$ wsl --list --online
$ wsl --install -d Ubuntu
```
3. Download and Install Docker Desktop
