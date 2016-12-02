### Ubuntu-Git-Java-8-Maven-Hadoop-Hive-Docker-Image ###
> Docker image having Ubuntu Git Java-8 Maven hadoop Hive.

## Version ##
* Ubuntu Latest
* Git Latest
* Oracle Java 8
* Maven Latest
* Apache Hadoop - 2.7.2
* Apache Hive - 2.1.0

## Setup ##
1. Install [docker](https://www.docker.com/products/overview "Install Docker")
2. Execute to start Hive CLI `docker run -it goyalzz/ubuntu-git-java-8-maven-hadoop-hive-docker-image /bin/bash -c 'cd /usr/local/hive && ./bin/hive'`

## Test Hive ##
- create database sample;
- use sample;
- create table product(product int, productname string, price float);
- describe product;
- select * from product;

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