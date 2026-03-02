# CI/CD Pipeline using Jenkins & Docker

## Project Overview

This project demonstrates how a simple web application can be automatically built and deployed using a CI/CD pipeline.  
Whenever code is pushed to the GitHub repository, Jenkins automatically pulls the latest code, builds a Docker image and runs the application inside a container on an AWS EC2 instance.

The objective of this project is to understand real-world DevOps practices such as automated builds, containerization and continuous deployment.

---

## Technologies Used

Jenkins for pipeline automation  
Docker for containerization  
Git and GitHub for source code management  
AWS EC2 Amazon Linux instance as the build and deployment server  
Nginx as the web server inside the Docker container

---

## How the Pipeline Works

The pipeline performs the following steps automatically.

First, Jenkins connects to the GitHub repository and checks out the latest code.  
Next, a Docker image is built using the Dockerfile present in the repository.  
After that, any previously running container of the same application is removed.  
Finally, a new container is started and the application becomes available to users.

---

## Application Access

After a successful pipeline execution, the application can be accessed from a browser using

http://<EC2-PUBLIC-IP>:8090

---

## Repository Structure
