# RabbitMQ 
Based on the following repo: https://github.com/spring2/dockerfiles/tree/master/rabbitmq

RabbitMQ running in windows container with:
- Basic install with default guest enabled
- Remote host access is enabled.
- AMQP 1.0 plugin enabled


build:
```
docker build --build-arg VERSION=3.6.15 -t <image name> .
```

run:
```
docker run -d --name rabbitmq <image name>
```


view enabled plugins:
```
docker exec -it rabbitmq cmd /c rabbitmq-plugins list
```

ToDo:
- use ENV vars to set default username and password
- example of VOLUME mapped directory
"# rabbitmq-windows-container" 
