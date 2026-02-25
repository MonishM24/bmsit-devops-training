```
docker version
docker info
docker
docker container run
docker run
docker search ubuntu
docker pull ubuntu
docker run ubuntu


docker container run --publish 80:80 nginx
docker container run --publish 80:80 --detach nginx
docker container ls
docker container stop 
docker container ls
docker container ls -a
docker container run --publish 80:80 --detach --name webhost nginx
docker container run -d -p 3306:3306 --name db -e MYSQL_RANDOM_ROOT_PASSWORD=yes mysql

docker container run -d --name db -e MYSQL_RANDOM_ROOT_PASSWORD=true mysql

docker container run -it --name webserver nginx bash

docker container run --publish 80:80 --detach --name webhost nginx
docker container logs webhost
docker container top webhost
docker container run -d --name mysql -e MYSQL_RANDOM_ROOT_PASSWORD=true mysql
docker container inspect mysql
docker container stats mysql
```

