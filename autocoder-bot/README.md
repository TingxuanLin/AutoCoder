# Python Web Service
## Project Setup
The project is a containerized Python web service. It uses a multi-stage Docker build for a lightweight final image.
## Building and Running the Container
1. Build the Docker image by running `docker build -t python-web-service .` in the root directory.
2. Run the container with `docker run -p 5000:5000 python-web-service`.
## Dependencies
The project depends on Flask, which is listed in the `requirements.txt` file.
