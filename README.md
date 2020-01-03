# Docker based Nginx testing steps --> Nginx is webserver, caching tool and loadbalancer

Docker Hello World Example
--------------------------
docker run hello-world

#  docker build -t radhed/rrnginx ../ --> localtion should be root of Dockerfile

# docker run --name rrnginxserver4 -d -p 8081:9080 radhed/rrnginx

# docker run --name rrnginxserver2 -d -p 8080:80 radhed/rrnginx

List Docker process
-----------------------
docker ps
docker ps -a

Remove containers by name
-----------------------------
docker rm <name>

Kill running container
-------------------------------
docker kill <container_id>

List cached container images
------------------------------
docker images

Check logs for Containers
----------------------------
docker logs <container_id>

