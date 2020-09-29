# DockerLearnings

### Essential commands
Pull a ubuntu image from Docker Hub
```
docker pull ubuntu
```
Search local images
```
docker images
```
Spin up a container from the ubuntu image and run the bash process on it. Here -ti = terminal interactive (Creates a readable output on the terminal)
```
docker run -ti ubuntu bash
```
Display containers that are currently running
```
docker ps
```
Stop a container
```
docker kill container-id
```
Create an image out of the stopped container and tag it
```
docker commit container-id my-image
```
Spin up a detached docker container which runs in the background
```
docker run -d -ti ubuntu bash
```
Spin up a temporary docker container which kills itself at the end of the process execution
```
docker --rm run -ti ubuntu sleep 5
```
Attach the detached docker container
```
docker attach container-id
```
Execute a second process in an already running docker container
```
docker exec container-id bash
```


