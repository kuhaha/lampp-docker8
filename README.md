# LAMPP on Docker
1. Download and Install [Docker Desktop](https://www.docker.com/products/docker-desktop/)
2. Download & Unzip or Clone the repository, in folder such as `c:\dev\lampp-docker8`
    - `$ cd c:\dev\lampp-docker8`
4. Run `docker-compose` command
    - `$ docker-compose up -d`
5. Open browser and view top pages
    - `http://localhost` (web home)
    - `http://localhost:8080` (phpmyadmin)


# How to Install Docker Desktop 

## Install Docker Desktop on Windows Machine
1. Enable Virtualization at BIOS
2. Open WSL terminal
3. Update WSL 
  - `$ wsl.exe --update`
3. Check Linux distributions available online
  ```sh
$ wsl.exe --list --online
NAME                            FRIENDLY NAME
Ubuntu                          Ubuntu
Debian                          Debian GNU/Linux
kali-linux                      Kali Linux Rolling
Ubuntu-18.04                    Ubuntu 18.04 LTS
Ubuntu-20.04                    Ubuntu 20.04 LTS
Ubuntu-22.04                    Ubuntu 22.04 LTS
Ubuntu-24.04                    Ubuntu 24.04 LTS
OracleLinux_7_9                 Oracle Linux 7.9
OracleLinux_8_7                 Oracle Linux 8.7
OracleLinux_9_1                 Oracle Linux 9.1
openSUSE-Leap-15.6              openSUSE Leap 15.6
.....
```
4. Choose and install a Linux distribution
  - `$ wsl.exe --install -d Ubuntu`
5. Download and Install Docker Desktop

## Install Docker Desktop on Linux Machine
1. Enable `centos-extras`
  - `$ sudo yum install epel-release`
2. Setup Repository
  - ```
$ sudo yum install -y yum-utils \
  device-mapper-persistent-data \
  lvm2
```
3. Install Docker Engine
  - `$ sudo yum install docker-ce`

# How to Connect to MySQL in PHP

- `$conn = new mysqli("mysql",<user>,<passwd>, <db_name>);`
    - user accounts (userid/passwd): `root`/`root`, `test`/`test`     

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
