# Project Setup
This is a basic Python web service setup using Docker for containerization.

## Prerequisites
- Docker installed on your system
- Basic knowledge of Docker and Python

## Building the Docker Image
1. Navigate to the project directory.
2. Run the command `docker build -t my-python-service .` to build the Docker image.

## Running the Docker Container
1. Run the command `docker run -p 5000:5000 my-python-service` to start a new container from the image.
2. Access the web service at `http://localhost:5000`.
