# Jenkins Docker CI/CD Project

## Project Overview

This project demonstrates a CI/CD pipeline using Jenkins and Docker to build and deploy a Java Maven web application.

The application is built using Maven, packaged as a WAR file, converted into a Docker image using Apache Tomcat, and deployed as a Docker container on an AWS EC2 instance.

## Tools Used

- Git & GitHub
- Jenkins
- Maven
- Docker
- Apache Tomcat
- AWS EC2
- Linux

## CI/CD Pipeline Stages

1. **Checkout Code**
   - Pulls source code from GitHub.

2. **Compile Project**
   - Compiles the Maven project.

3. **Build Artifact**
   - Creates the WAR file using Maven.

4. **Build Docker Image**
   - Builds a Docker image using the Dockerfile.

5. **Deploy Container**
   - Stops the old container.
   - Removes the old container.
   - Runs the new container on port 9090.

## Docker Deployment

The application runs inside a Tomcat Docker container.

Browser URL:

```text
http://<EC2-PUBLIC-IP>:9090/maven-web-app/
