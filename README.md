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
