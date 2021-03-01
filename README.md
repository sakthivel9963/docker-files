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
  - ```sh
    docker-compose -f mysql.yml up -d
    ```
