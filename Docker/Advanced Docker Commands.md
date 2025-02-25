# Advanced Docker Commands

## Building Docker Images

### Build an image from a Dockerfile:
docker build -t my-image:latest .

### Build an image with no cache:
docker build --no-cache -t my-image:latest .

### Build an image and specify a build argument:
docker build --build-arg VAR_NAME=value -t my-image:latest .

---

## Running Containers

### Run a container in detached mode:
docker run -d --name my-container my-image:latest

### Run a container with an interactive shell:
docker run -it --name my-container my-image:latest /bin/bash

### Run a container and expose ports:
docker run -d -p 8080:80 --name my-container my-image:latest

### Run a container with an environment variable:
docker run -e MY_ENV_VAR=value -d --name my-container my-image:latest

### Run a container and mount a volume:
docker run -v /host/path:/container/path -d --name my-container my-image:latest

---

## Inspecting Containers and Images

### List running containers:
docker ps

### List all containers (including stopped ones):
docker ps -a

### Get detailed information about a container:
docker inspect my-container

### Get the environment variables of a running container:
docker exec my-container env

### Get the logs of a container:
docker logs my-container

### Check the port mappings of a container:
docker port my-container

### Show resource usage of running containers:
docker stats

---

## Managing Containers

### Stop a running container:
docker stop my-container

### Start a stopped container:
docker start my-container

### Restart a container:
docker restart my-container

### Remove a container:
docker rm my-container

### Remove all stopped containers:
docker container prune

---

## Managing Images

### List images:
docker images
# Advanced Docker Commands

## Building Docker Images

### Build an image from a Dockerfile:
docker build -t my-image:latest .

### Build an image with no cache:
docker build --no-cache -t my-image:latest .

### Build an image and specify a build argument:
docker build --build-arg VAR_NAME=value -t my-image:latest .

---

## Running Containers

### Run a container in detached mode:
docker run -d --name my-container my-image:latest

### Run a container with an interactive shell:
docker run -it --name my-container my-image:latest /bin/bash

### Run a container and expose ports:
docker run -d -p 8080:80 --name my-container my-image:latest

### Run a container with an environment variable:
docker run -e MY_ENV_VAR=value -d --name my-container my-image:latest

### Run a container and mount a volume:
docker run -v /host/path:/container/path -d --name my-container my-image:latest

---

## Inspecting Containers and Images

### List running containers:
docker ps

### List all containers (including stopped ones):
docker ps -a

### Get detailed information about a container:
docker inspect my-container

### Get the environment variables of a running container:
docker exec my-container env

### Get the logs of a container:
docker logs my-container

### Check the port mappings of a container:
docker port my-container

### Show resource usage of running containers:
docker stats

---

## Managing Containers

### Stop a running container:
docker stop my-container

### Start a stopped container:
docker start my-container

### Restart a container:
docker restart my-container

### Remove a container:
docker rm my-container

### Remove all stopped containers:
docker container prune

---

## Managing Images

### List images:
docker images

### Remove an image:
docker rmi my-image:latest

### Remove all unused images:
docker image prune -a

---
### Remove an image:
docker rmi my-image:latest

### Remove all unused images:
docker image prune -a

---
