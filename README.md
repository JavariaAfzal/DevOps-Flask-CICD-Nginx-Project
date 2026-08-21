# DevOps-Flask-CICD-Nginx-Project

Complete DevOps CI/CD project using Python Flask, GitHub Actions, Docker, Nginx, and Render.

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_



#### Project Overview



This project demonstrates a complete DevOps workflow for deploying a Python Flask web application.



The project covers application development, containerization, reverse proxy configuration, CI/CD automation, and cloud deployment.

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_



#### &#x20;Technologies Used



\- Python

\- Flask

\- Gunicorn

\- Docker

\- Nginx

\- Git

\- GitHub

\- GitHub Actions

\- Render

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_



#### Project Architecture



Developer

&#x20;  ↓

GitHub Repository

&#x20;  ↓

GitHub Actions CI/CD Pipeline

&#x20;  ↓

Docker Image

&#x20;  ↓

Flask Application

&#x20;  ↓

Gunicorn

&#x20;  ↓

Nginx Reverse Proxy

&#x20;  ↓

Cloud Deployment

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_



##### &#x20;Application:-



The application is built using Python Flask.



Flask provides the web application, while Gunicorn is used as the production WSGI server.



##### &#x20;Docker:-



The Flask application is containerized using Docker.



Docker packages the application together with its dependencies so that it can run consistently across different environments.



The Docker image is built using the project's `Dockerfile`.



##### &#x20;Gunicorn:-



Gunicorn is used instead of Flask's development server for production-style execution.



It runs the Flask application as a WSGI application and provides a more suitable application server for deployment.



##### &#x20;Nginx:-



Nginx is configured as a reverse proxy in front of the Flask application.



It receives incoming HTTP requests and forwards them to the Flask application running behind Gunicorn.



##### &#x20;CI/CD Pipeline:-



GitHub Actions is used to automate the CI/CD workflow.



Whenever changes are pushed to the repository, the workflow runs automatically and verifies the project.



The pipeline helps automate the process instead of manually checking every change.



##### &#x20;Local Docker Setup:-



The Flask application can be built using:



docker build -t devops-flask-app .\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_



##### &#x20;Project Structure:



DevOps-Flask-CICD-Nginx-Project/

├── .github/

│   └── workflows/

│       └── ci.yml

├── nginx/

│   └── nginx.conf

├── app.py

├── Dockerfile

├── requirements.txt

└── README.md



