# Base Alpine Linux based image with OpenJDK JRE only
FROM openjdk:8-jre-alpine
EXPOSE 8080
# copy application WAR (with libraries inside)
COPY helloworld-0.0.1-SNAPSHOT.jar /app.jar
# specify default command
CMD ["/usr/bin/java", "-jar", "-Dspring.profiles.active=dev", "/app.jar"]
