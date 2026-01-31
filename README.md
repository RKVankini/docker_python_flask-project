# Dockerized Python Flask Application

A simple Python Flask web application containerized using Docker.
This project demonstrates how to build, package, and run a Flask application inside a Docker container.

## Project Overview

This repository contains a lightweight Flask application that is:
- Written in Python
- Containerized using Docker
- Portable and easy to deploy on any Docker-enabled system

This project is intended for learning Docker fundamentals and basic DevOps workflows.

## Technologies Used

- Python 3
- Flask
- Docker
- Git & GitHub

## Project Structure

#.
#├── app.py
#├── requirements.txt
#├── Dockerfile
#├── README.md

## Prerequisites

Ensure the following tools are installed on your system:
- Docker
- Git

## How to Run the Application

1. Clone the repository

git clone https://github.com/RKVankini/docker-python-flask-app.git
cd docker-python-flask-app

2. Build the Docker image

docker build -t simple-flask-app:latest .

3. Run the Docker container

docker run -d -p 5000:5000 simple-flask-app

## Access the Application

Open a web browser and navigate to:

http://127.0.0.1:5000

If Docker is running inside a virtual machine, use the VM IP address:

http://<VM_IP>:5000

## Learning Outcomes

- Understanding Dockerfile structure
- Building Docker images
- Running containers for Python applications
- Exposing container ports to host systems

## Future Enhancements

- Production deployment using Gunicorn
- Reverse proxy using Nginx
- CI/CD pipeline using GitHub Actions
- Cloud deployment on AWS

## Author

Rama Krishna Vankini  
AWS | Docker | DevOps Enthusiast

## License

This project is open for learning and educational purposes.
