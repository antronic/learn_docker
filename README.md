# learn_docker
Try to use docker for better life :D
## First Step!
- We have to create ```Dockerfile``` first!
- We place ```Dockerfile``` in a same directory with out project, you can see from this repository.

  ### Example of Dockerfile
  ```dockerfile
  # FROM <image from repositories>
  FROM php:7.0-apache
  # COPY is command to copy files from local computer to DockerImage
  COPY src/ /var/www/html
  # EXPOSE is command to use port 80 by default
  EXPOSE 80
  ```
  You can find more repositories from [hub.docker.com]('https://hub.docker.com/')

## Second Step!
  - We have to use command to do something.
  - After we create a Dockerfile, we need to build it by using following command below.
  ## Simple Command
  #### build an image from Dockerfile
  ```bash
  $ docker build -t hello-docker #<path to DockerFile>
  ```
