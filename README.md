# docker
Docker Repository for practice

## Installation Steps
```
1. Go to https://docs.docker.com/engine/install/ubuntu/
2. Copy all commands together from
    1. Set up docker apt repo
    2. Install docker
    3. Start service
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
