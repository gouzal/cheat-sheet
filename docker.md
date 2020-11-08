## Template Format for Java/Spring   
```java <!-- Just for syntax highlighting -->
FROM openjdk:11
ADD target/JDock.jar JDock.jar
EXPOSE 8080
ENTRYPOINT [ "java","-jar","JDock.jar" ]
```
