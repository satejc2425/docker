# docker
Docker Repository for practice
#Installation Steps
```
1. Go to https://docs.docker.com/engine/install/ubuntu/
2. Copy all commands together from
    1. Set up docker apt repo
    2. Install docker
    3. Start service
```
# Docker Commands

docker version --> checks if docker is working or not

docker images
docker pull nginx:latest --> Downloads an image
docker images 

docker run --name test -d -p 8080:80 nginx:latest --> starts container from image and then go to browser and browse localhost:8080
docker ps --> shws details about containers

docker exec -it test /bin/bash --> Execute a command inside a container
ls 
exit

docker ps
docker stop test
docker rm test --> Delete container
docker ps -a
