Docker Calculator — Python

A simple Python command-line calculator packaged inside a Docker container.
This project demonstrates how to:

write a basic Python program

create a Dockerfile

build a Docker image

run the app inside a container

Great for beginners learning Docker + Python together.

🔧 Project Structure
Docker-Project1/
│
├── calculator.py
└── dockerfile


# Docker Setup

Build the Docker Image

Run inside the project folder:

docker build -t vishnuj1999/first-docker-image:latest .


Note the space before the dot (.).

# Run the Container
docker run -it vishnuj1999/first-docker-image:latest


-it lets you interact with the calculator inside the container.

# Example Dockerfile

(Your file should look similar to this)

FROM python:3.10-slim

WORKDIR /app

COPY calculator.py .

CMD ["python", "calculator.py"]

<img width="1190" height="521" alt="docker container" src="https://github.com/user-attachments/assets/e6f541fa-e500-4bbd-b9a3-246b25814253" />
<img width="1560" height="765" alt="docker-image" src="https://github.com/user-attachments/assets/b36bb54e-58f0-41ed-bf42-baeb3f82b162" />

