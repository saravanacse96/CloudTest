# Step 1: Use a base image with Java
FROM openjdk:17-jdk-slim

# Step 2: Set a working directory in the container
WORKDIR /src

# Step 3: Copy the JAR file to the container
COPY target/CloudTest-0.0.1-SNAPSHOT.jar  app.jar

# COPY build/libs/myapp.jar app.jar  # For Gradle

# Step 4: Expose the port your app runs on
EXPOSE 8080

# Step 5: Run the application
ENTRYPOINT ["java", "-jar", "app.jar"]
