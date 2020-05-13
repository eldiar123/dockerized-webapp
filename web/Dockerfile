FROM openjdk:8-jdk-alpine

ADD webapp/target/webapp.jar app.jar

EXPOSE 8080

#ENTRYPOINT [ "sh", "-c", "java -jar /app.jar"]
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-Dspring.profiles.active=container", "-jar", "app.jar"]
