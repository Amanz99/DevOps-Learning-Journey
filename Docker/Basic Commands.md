# Docker Commands Summary

## 1. Running a Container  
- **`docker run <image>`**: Runs a container from an image.  
  - If the image is not available locally, it pulls it from Docker Hub (only the first time).  

## 2. Viewing Running Containers  
- **`docker ps`**: Lists all running containers.  
- **`docker ps -a`**: Lists all containers, including stopped ones.  

## 3. Stopping and Removing Containers  
- **`docker stop <container_id/name>`**: Stops a running container.  
- **`docker rm <container_id/name>`**: Permanently removes a stopped container.  

## 4. Managing Images  
- **`docker images`**: Lists available images on the host.  
- **`docker rmi <image>`**: Removes an unused image (only if no containers depend on it).  
- **`docker pull <image>`**: Downloads an image without running it.  

## 5. Container Lifecycle  
- Running an Ubuntu container (`docker run ubuntu`) exits immediately because there’s no running process.  
- **`docker run ubuntu sleep 5`**: Runs Ubuntu and executes the sleep command for 5 seconds before exiting.  

## 6. Executing Commands in Containers  
- **`docker exec <container_id/name> <command>`**: Runs a command inside a running container.  

## 7. Foreground vs. Detached Mode  
- **`docker run <image>`**: Runs in the foreground, showing logs and output.  
- **`docker run -d <image>`**: Runs in detached mode (background).  
- **`docker attach <container_id/name>`**: Reattaches to a running container.  


