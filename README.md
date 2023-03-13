# Docker File

## Install Docker compose

```sh
sudo apt install docker-compose
```

## Running docker file in the terminal

- ```sh
  docker-compose -f filename up
  ```
- ```sh
  docker-compose -f mysql.yml up
  ```
- ### Running docker in the background add **-d** in the command

  ```sh
  docker-compose -f mysql.yml up -d
  ```

- ### start service
  ```sh
  docker-compose container-name start
  ```
- ### stop service
  ```sh
  docker-compose container-name stop
  ```
- ### stop service and remove service
  ```sh
  docker-compose container-name down
  ```
- ### stop service with file name
  ```sh
  docker-compose -f mysql.yml stop
  ```
- ### stop service and remove service with file name
  ```sh
  docker-compose -f mysql.yml down
  ```
- ### list all the container
  ```sh
  docker ps
  ```
  ```sh
  docker container ls
  ```
- ### list all the images
  ```sh
  docker image ls
  ```
- ### remove container from docker
  ```sh
  docker rm container-name or container-id
  ```
- ### remove image from docker
  ```sh
  docker image rm image-name or image-id
  ```
- ### Build project from the docker file
  ```sh
  docker build -t your_docker_hub_username/nodejs-image-demo .
  ```
  The **( . )dot** specifies that the build context is the current directory.
  The **your_docker_hub_username** we can specify it or just leave it.
  ```
  docker build -t nodejs-express-image .
  ```
- ### Run the build docker image
  ```sh
  docker run --name nodejs-image-demo -p 80:8080 -d your_docker_hub_username/nodejs-image-demo
  ```
  The **--name** tag is optional and this allows you to give the container name.
  ```sh
  docker run -p 3050:3050 -d nodejs-express-image
  ```
- ### Print container log
  ```sh
  docker logs container_id
  ```
