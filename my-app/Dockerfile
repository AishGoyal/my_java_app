# Use an official Maven image with JDK 11 (or adjust the version as needed)
FROM maven:3.8.5-openjdk-11-slim

# Set the working directory inside the container
WORKDIR /app

# Copy the pom.xml file and the source code into the container
COPY pom.xml .
COPY src ./src

# Run Maven build and tests
RUN mvn clean package

# Specify the entry point command to run your application
# Adjust the JAR file name if necessary
ENTRYPOINT ["java", "-jar", "target/my-app-1.0-SNAPSHOT.jar"]
