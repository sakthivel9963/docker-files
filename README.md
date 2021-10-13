# Docker Files

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
- ### list all the images
  ```sh
  docker images
  ```
- ### remove container from docker
  ```sh
  docker rm container-name or container-id
  ```
- ### remove image from docker
  ```sh
  docker image rm image-name or image-id
  ```
