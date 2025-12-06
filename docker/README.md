### Build Docker image
```docker build -t springboot-app .```
### Build image from current folder Dockerfile

### See all images
```docker images```
### List all Docker images

### Run container
```docker run -d -p 7071:7070 --name springboot-1 springboot-app```
### Run container in background, map host 7071 → container 7070

### See running containers
```docker ps```
### Show all running containers

### Stop container
```docker stop springboot-1```
### Stop a running container

### Remove container
```docker rm springboot-1```
### Delete container to reuse name

### Check container logs
```docker logs springboot-1```
### See Spring Boot logs

### Run multiple containers from same image
```docker run -d -p 7072:7070 --name springboot-2 springboot-app```
```docker run -d -p 7073:7070 --name springboot-3 springboot-app```
### Multiple instances with different host ports & unique names

### Stop all running containers (shortcut)
```docker stop $(docker ps -q)```
### Stops all running containers

### Remove image
```docker rmi springboot-app```
### Delete the Docker image