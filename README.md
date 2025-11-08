# project1
deploying a Dockerized application on kubernete.

## Description
This project demonstrates a simple web application deployment process using Docker, Kubernetes, and GitHub.
It includes creating a Docker image for a web app, pushing it to Docker Hub, and deploying it on a Kubernetes cluster.

## Technologies Used
HTML – for the frontend page (index.html)
Docker – for containerizing the web application
Kubernetes (kubectl) – for managing deployment and service
Git & GitHub – for version control

## Initialize Git and push code to GitHub
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/dara123-gif/project1.git
git branch -M main
git push -u origin main

## Create index page and Dockerfile
vi index.html
vi Dockerfile
git add .
git commit -m "Created index page and Dockerfile"

## Build and push Docker image
docker build -t dara123-gif/web:v1 .
docker push dara123-gif/web:v1

## Create and apply Kubernetes deployment
vi dep.yaml
kubectl apply -f dep.yaml
kubectl get svc
