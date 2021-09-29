FROM openjdk:8-jdk-alpine
EXPOSE 8080
ADD target/hello-0.0.1-SNAPSHOT.jar hello-0.0.1-SNAPSHOT.jar
ENTRYPOINT ["sh", "-c", "java -jar /hello-0.0.1-SNAPSHOT.jar"]