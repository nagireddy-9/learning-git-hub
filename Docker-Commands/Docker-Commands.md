##ISTALL DOCKER ON UBUNTU
*  install the docker on ubuntu machine
   ```
   sudo apt-get update
   sudo apt-get install docker.io
   sudo usermod -aG docker ubuntu
   ```
* create an image build from Dockerfile
  ```
  docker build -t jenkins:latest Dockerfile
  docker image ls
  docker inspect jenkins
  ```   
* create a container from above build image
 ```
 docker run -d -it --name jenkins-container -p 8081:8080 image-name
 ```
* To enter inside that container use bellow command
 ```
 docker exec -i container-name /bin/bash
 ```
* To find ip of container
 ```
 docker inspect $(docker ps -q) | grep IPAdderess
 ``` 