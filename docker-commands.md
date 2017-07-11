#Running containers
docker ps
#Running + stopped containers
docker ps -a
#Getting all the id of containers
docker ps -a -q
#Getting all the id of images
docker images -q
#Deleting all containers from docker host
docker rm `docker ps -a -q`
#Deleting all images from docker host
docker rmi `docker images -q`
#List all the images
docker images ls


#Running rabbit-mq locally
With Management Plugin
docker run -d --hostname my-rabbit --name some-rabbit1 -p 8080:15672 -p 5672:5672 rabbitmq:3-management

#Running rabbit-mq locally with lastest without management plugin
docker run -d --hostname my-rabbit --name some-rabbit1  -p 5672:5672 rabbitmq:latest