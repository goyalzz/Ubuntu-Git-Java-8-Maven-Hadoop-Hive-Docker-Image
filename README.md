### Ubuntu-Git-Java-8-Maven-Spring-Tool-Suit-Docker-Image ###
> This project is a simple Docker image that runs the [Spring Tool Suite IDE]().

## Version ##
* Ubuntu Latest
* Git Latest
* Oracle Java 8
* Maven Latest
* STS - 3.8.4.RELEASE

## Setup ##
1. Install [docker](https://www.docker.com/products/overview "Install Docker")
2. Execute to start Hive CLI `docker run -it goyalzz/Ubuntu-Git-Java-8-Maven-Spring-Tool-Suit-Docker-Image /bin/bash`

## Prerequisites ##
* a working [Docker](http://docker.io) engine
* a working [Docker Compose](http://docker.io) installation

## Building ##
Type `docker-compose build` to build the image.

## Installation ##
Docker will automatically install the newly built image into the cache.

## Tips and Tricks ##

## Launching The Image ##

`docker-compose up` will launch the image allowing you to begin working on projects. The Docker Compose file is 
configured to mount your home directory into the container.  

## User Account ##
The image assumes that the account running the continer will have a user and group id of 1000:1000.  This allows the container 
to save files in your home directory and keep the proper permissions.

## X-Windows ##
If the image complains that it cannot connect to your X server, simply run `xhost +` to allow the container to connect 
to your X server.

# Some useful docker comands #
1.  `docker search ubuntu/java`
2.  `docker images -a`
3.  `docker ps -a`
4.  `exit`
5.  `docker run -it <Image>`
6.  `docker rm -f $(docker ps -a -q)`
7.  `docker rmi -f $(docker images -a -q)`
8.  `docker tag <image> <new name>`
9.  `docker build -f Dockerfile -t <image name> .`
10. `touch Dockerfile`
11. `docker exec -it <CONTAINER_ID> /bin/bash`
