## Install Docker

```
dhclient
yum install docker
```

## Start Docker Service

```
service docker start
```

## List all images

```
docker images
```

## Run a container
```
docker run hello-world
```
This will pull the image from dockerhub and then run.

## Pull image from dockerhub and run
```
docker pull busybox
docker run busybox
```

## Run docker container in interactive mode
```
docker run -it busybox sh
```

## Display running docker containers
```
docker ps
```

## Display all docker containers
```
docker ps -a
```

## Display process ids of all docker containters
```
docker ps -a -q 
```

## Display process ids of all docker containters with Filter
```
docker ps -a -q -f status=exited
```

## Remove a exited container```
```
docker ps hello-world
```

## Remove a running container
```
docker stop $(docker ps -a -q)
docker rm $(docker ps -a -q)
```



