# Docker Foundations Assignment

This repository contains hands-on Docker fundamentals and practical assignments completed as part of my DevOps learning journey.

The project demonstrates core Docker concepts including:
- Docker installation
- Docker images
- Docker containers
- Dockerfile creation
- Port mapping
- Container lifecycle management
- Basic application containerization

---

# Project Objective

The main objective of this assignment is to understand and implement Docker fundamentals used in DevOps and cloud environments.

This project helps in learning:
- What Docker is and how it works
- Difference between Docker Images and Containers
- How to create custom Docker images
- How to run applications inside containers
- Container management and networking basics

---

# Technologies Used

- Docker
- Linux
- Ubuntu
- Git
- GitHub

---

# Docker Concepts Covered

## 1. Docker Installation

Installing Docker on Ubuntu/Linux environment.

### Verify Docker Installation
```bash
docker --version
```

---

## 2. Docker Images

Pulling Docker images from Docker Hub.

### Example
```bash
docker pull nginx
```

### View Docker Images
```bash
docker images
```

---

## 3. Docker Containers

Running and managing Docker containers.

### Run Nginx Container
```bash
docker run -d -p 80:80 nginx
```

### Check Running Containers
```bash
docker ps
```

### Check All Containers
```bash
docker ps -a
```

---

## 4. Dockerfile

Creating custom Docker images using Dockerfile.

### Sample Dockerfile
```Dockerfile
FROM ubuntu

RUN apt update

CMD ["echo", "Docker Foundations Assignment"]
```

---

## 5. Build Docker Image

Building Docker image from Dockerfile.

```bash
docker build -t myapp .
```

---

## 6. Run Custom Docker Image

```bash
docker run myapp
```

---

## 7. Port Mapping

Exposing container ports to host machine.

### Example
```bash
docker run -d -p 8080:80 nginx
```

Where:
- 8080 = Host machine port
- 80 = Container port

---

## 8. Container Management

### Stop Container
```bash
docker stop container_id
```

### Start Container
```bash
docker start container_id
```

### Restart Container
```bash
docker restart container_id
```

### Remove Container
```bash
docker rm container_id
```

---

# Repository Structure

```bash
docker-foundations-assignment/
│
├── Dockerfile
├── README.md
├── app/
├── screenshots/
└── commands/
```

---

# Common Docker Commands

## Check Docker Version
```bash
docker --version
```

## Pull Docker Image
```bash
docker pull nginx
```

## List Docker Images
```bash
docker images
```

## Run Docker Container
```bash
docker run -d -p 8080:80 nginx
```

## List Running Containers
```bash
docker ps
```

## List All Containers
```bash
docker ps -a
```

## Stop Container
```bash
docker stop container_id
```

## Remove Container
```bash
docker rm container_id
```

## Remove Docker Image
```bash
docker rmi image_id
```

---

# Learning Outcomes

After completing this assignment, I learned:
- Docker fundamentals
- Containerization concepts
- Docker image creation
- Dockerfile usage
- Port mapping
- Docker container lifecycle
- Basic DevOps workflow

---

# Real-World Use Cases of Docker

Docker is widely used for:
- Application deployment
- Microservices architecture
- CI/CD pipelines
- Cloud-native applications
- Environment consistency
- Faster software delivery

---

# Future Improvements

Future enhancements planned for this project:
- Docker Compose implementation
- Multi-container applications
- CI/CD pipeline integration
- Kubernetes deployment
- AWS EC2 deployment
- Monitoring and logging setup

---

# Author

## Mustafa Balasinorwala

DevOps Enthusiast

GitHub:
https://github.com/MustafaBalasinorwala91

---

# Conclusion

This assignment provided practical experience with Docker and containerization concepts used in DevOps, Cloud Computing, and modern application deployment environments.

It helped in understanding how Docker simplifies application deployment, improves portability, and ensures consistency across different environments.
