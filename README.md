# Docker
Containerization of java app project using Docker

This is a project on how to containerize a java project using docker.

### BENEFITS:
- If you can containerize an application, then you can save a lot of money
- It consumes low resources
- Suits very well for microservice design
- Deployment are done via image
- Same container images across environment
- Reusable and repeatable

### TOOLS:
- Docker (Container runtime environment)
- Java stack (Application services)
- Maven
- Docker compose(To test run the built images)

### STEPS
- Find right base image from dockerhub
- Write dockerfile to customize images
- Write docker compose.yaml file to run multi containers

### ARCHITECTURE EXPLAINED:
First we fetch our source code from git repository. We then write a docker file for the service that needs customization(NGINIX, TOMCAT, MYSQL) I.e we write 3 dockerfiles. We use docker build command which will get executed on our docker engine. The 3 services will be pulled from dockerhub.

Docker build command is going to read the docker file, build our image and once our images are ready, we are going to use docker compose. Once it checks out fine, then we are going to push our containerized docker images to our dockerhub account.
