## Template Format for Java/Spring   
```java <!-- Just for syntax highlighting -->
FROM openjdk:11
ADD target/JDock.jar JDock.jar
EXPOSE 8080
ENTRYPOINT [ "java","-jar","JDock.jar" ]
```

Procedure
Stop the container(s) using the following command:
docker-compose down
Delete all containers using the following command:
docker rm -f $(docker ps -a -q)
Delete all volumes using the following command:
docker volume rm $(docker volume ls -q)
Restart the containers using the following command:
docker-compose up -d
