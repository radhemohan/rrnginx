# Docker based Nginx testing steps --> Nginx is webserver, caching tool and loadbalancer

Docker Hello World Example
--------------------------
docker run hello-world

Build new Docker image using Nginx server as Base
------------------------------------------------
 docker build -t radhed/rrnginx ../ --> localtion should be root of Dockerfile

Run Nginx server and Expose server port as 9080(Check EXPOSE command in Dockerfile)
------------------------------------------------
docker run --name rrnginxserver4 -d -p 8081:9080 radhed/rrnginx


Run Nginx Server on 80 and expose external posr as 8080
-------------------------------------------------------
docker run --name rrnginxserver2 -d -p 8080:80 radhed/rrnginx

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

