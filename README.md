# Simple Python Flask Dockerized Application

This repository contains a simple Python Flask application that is Dockerized for easy setup and deployment.

This is my customized version of a basic Flask + Docker project, created for learning and practicing Docker, containerization, and DevOps fundamentals.

## Build the Docker Image

Build the Docker image using the following command:

```bash
docker build -t simple-flask-app:latest .
Run the Docker Container
Run the Docker container using the command shown below:
docker run -d -p 5000:5000 simple-flask-app

Access the Application

The application will be accessible at:
http://127.0.0.1:5000

If you are using boot2docker, first find the IP address using:
docker run -d -p 5000:5000 simple-flask-app

Then access the application using:
http://<host_ip>:5000

Dockerfile
# Use the official Python 3.6 image from Docker Hub
FROM python:3.6

# Set the maintainer label
MAINTAINER Rama Krishna "ramakrishnavankini23@gmail.com"

# Copy the current directory contents into the /app directory in the container
COPY . /app

# Set the working directory to /app
WORKDIR /app

# Install any needed packages specified in requirements.txt
RUN pip install -r requirements.txt

# Set the entry point to python
ENTRYPOINT ["python"]

# Run app.py when the container launches
CMD ["app.py"]


Project Purpose

This project demonstrates how to Dockerize a Python Flask application and run it inside a Docker container.

Technologies Used

Python

Flask

Docker

Author

Rama Krishna Vankini
AWS | Docker | DevOps Learner



<!-- # Simple Python Flask Dockerized Application#

Build the image using the following command

```bash
$ docker build -t simple-flask-app:latest .
```

Run the Docker container using the command shown below.

```bash
$ docker run -d -p 5000:5000 simple-flask-app
```

The application will be accessible at http:127.0.0.1:5000 or if you are using boot2docker then first find ip address using `$ boot2docker ip` and the use the ip `http://<host_ip>:5000`


# Use the official Python 3.6 image from the Docker Hub
FROM python:3.6

# Set the maintainer label
MAINTAINER veera "veera.narni232@gmail.com"

# Copy the current directory contents into the /app directory in the container
COPY . /app

# Set the working directory to /app
WORKDIR /app

# Install any needed packages specified in requirements.txt
RUN pip install -r requirements.txt

# Set the entry point to python
ENTRYPOINT ["python"]

# Run app.py when the container launches
CMD ["app.py"] -->
