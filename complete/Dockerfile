# Start with a base image containing Java runtime
FROM openjdk:8-jdk-alpine

# Add Maintainer Info
LABEL maintainer="remi.castel1@epsi.fr"

# Add a volume pointing to /tmp
VOLUME /tmp

# Make port 8080 available to the world outside this container
EXPOSE 8090

# The application's jar file
ARG JAR_FILE=target/gs-spring-boot-docker-0.1.0.jar

COPY ${JAR_FILE} app.jar
ENTRYPOINT ["java","-jar","/app.jar"]