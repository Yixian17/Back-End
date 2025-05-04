# Use OpenJDK 17 as the base image
FROM openjdk:21

# Set the working directory inside the container
WORKDIR /app

# Copy the JAR file from the host into the container
ARG JAR_FILE=target/*.jar
COPY ${JAR_FILE} app.jar

# Run the application
ENTRYPOINT ["java", "-jar", "app.jar"]
