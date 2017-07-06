#Running rabbit-mq locally
With Management Plugin
docker run -d --hostname my-rabbit --name some-rabbit1 -p 8080:15672 -p 5672:5672 rabbitmq:3-management

#Running rabbit-mq locally with lastest without management plugin
docker run -d --hostname my-rabbit --name some-rabbit1  -p 5672:5672 rabbitmq:latest