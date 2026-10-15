# docker
Docker Repository for practice

## Installation Steps
1. Go to https://docs.docker.com/engine/install/ubuntu/
2. Copy all commands together from
   
1. Set up docker apt rep
```
       Add Docker's official GPG key:
       sudo apt update
       sudo apt install ca-certificates curl
       sudo install -m 0755 -d /etc/apt/keyrings
       sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc
       sudo chmod a+r /etc/apt/keyrings/docker.asc
            
       Add the repository to Apt sources:
       sudo tee /etc/apt/sources.list.d/docker.sources <<EOF
       Types: deb
       URIs: https://download.docker.com/linux/ubuntu
       Suites: $(. /etc/os-release && echo "${UBUNTU_CODENAME:-$VERSION_CODENAME}")
       Components: stable
       Architectures: $(dpkg --print-architecture)
       Signed-By: /etc/apt/keyrings/docker.asc
       EOF
            
       sudo apt update
```
   
2. Install docker
```
    sudo apt install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
```
3. Start service
```
    sudo systemctl status docker
    sudo systemctl start docker
```

# Docker Commands

1.docker version --> checks if docker is working or not

2.docker images
3.docker pull nginx:latest --> Downloads an image
4.docker images 

5.docker run --name test -d -p 8080:80 nginx:latest --> starts container from image and then go to browser and browse localhost:8080
6.docker ps --> shws details about all running containers

7.docker exec -it test /bin/bash --> Execute a command inside a container
8.ls 
9.exit

10.docker ps
11.docker stop test
12.docker rm test --> Delete container
13.docker ps -a
