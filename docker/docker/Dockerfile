# base image jdk
FROM eclipse-temurin:21-jdk
#FROM openjdk:21-jdk-slim


# working dir inside container
WORKDIR /app

# 3. Copy JAR file into container
COPY target/docker-0.0.1-SNAPSHOT.jar app.jar

# 4. Expose port (your Spring Boot port)
EXPOSE 7070

# 5. Run the JAR when the container starts
ENTRYPOINT ["java", "-jar", "app.jar"]



