## MEAN Stack Application – Dockerized Deployment with CI/CD
##  Project Overview
This project demonstrates end-to-end containerization and deployment of a MEAN (MongoDB, Express, Angular, Node.js) application using:

-Docker & Docker Compose

-MongoDB (Docker container)

-GitHub Actions CI/CD Pipeline

-Nginx Reverse Proxy

-Ubuntu Virtual Machine (AWS EC2)

The goal of this project is to showcase practical DevOps implementation including containerization, automation, and infrastructure setup.



## Project setup
## 1.Repository set up
-I have created new repository in my github

-Then pushed my code in to that repository from my local
## 2.Backend Dockerfile
-Created Dockerfile inside backend folder
<img width="802" height="277" alt="image" src="https://github.com/user-attachments/assets/28a04834-6b9b-4cda-a86b-859401ea68ca" />

## 3.Frontend Dockerfile
-Created Dockerfile inside the frontend folder
<img width="730" height="397" alt="image" src="https://github.com/user-attachments/assets/c7295725-58ec-4008-87b0-a13111e49bf0" />


## 4.Docker compose setup
-Created `docker-compose.yml` with services:

- mongodb
- backend
- frontend
- nginx

Used Docker Hub images for frontend & backend in production.

<img width="723" height="741" alt="image" src="https://github.com/user-attachments/assets/723815cb-8097-487c-b89c-331f0fdee4a4" />

## 5.Nginx Reverse Proxy Configuration
-Created nginx/default.conf




<img width="812" height="330" alt="image" src="https://github.com/user-attachments/assets/830ab66e-6264-44f9-824b-8d7c3ca10cf6" />









## 6.AWS EC2 Deployment
-Created EC2 Ubuntu instance

-Installed Docker & Docker Compose

-Cloned repository

-built and pushed the forntend and backend file to the docker hub

-Run the docker-compose file 

-Opened Port 80 in Security Group
## 7.CI/CD using GitHub Actions
-Trigger on push to main branch

-Build Docker images

-Push images to Docker Hub

-SSH into EC2

-Pull latest images

-Restart containers

<img width="977" height="806" alt="image" src="https://github.com/user-attachments/assets/4b8440be-5e94-465c-8a8c-5bc2dda5f196" />












## 8.GitHub Secrets Configured

DOCKER_USERNAME

DOCKER_PASSWORD

EC2_HOST

EC2_USER

EC2_SSH_KEY


  























