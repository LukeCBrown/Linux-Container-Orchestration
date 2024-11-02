# Rocky Linux Apache Web Server in Docker

This project sets up a simple Apache web server running in a Docker container with Rocky Linux 8. It's perfect as a quick-start example of Docker and demonstrates how to containerize a basic Linux service.

## Table of Contents
- [Overview](#overview)
- [Project Structure](#project-structure)
- [Prerequisites](#prerequisites)
- [Setup Instructions](#setup-instructions)
- [Usage](#usage)


## Overview
This repository contains a Dockerfile and sample HTML file that, together, allow you to run an Apache HTTP Server inside a Rocky Linux 8 container. The server serves a static HTML page on port 8080 of your local machine.

### Features
- Lightweight Rocky Linux 8 base image
- Apache HTTP Server installation and setup
- Basic HTML file served by Apache
- Port forwarding for local testing on `http://localhost:8080`


## Prerequisites
To run this project, ensure you have the following installed:
- **Docker**: You can install Docker by following the instructions [here](https://docs.docker.com/get-docker/).

## Setup Instructions
1. **Clone the Repository**  
   Clone this repository to your local machine:
   ```bash
   git clone https://github.com/yourusername/rockylinux-apache-docker.git
   cd rockylinux-apache-docker


## Building
```bash
docker build -t rockylinux-apache .
```
```bash
docker run -d -p 8080:80 rockylinux-apache
```

To stop the container, first list running containers to find the container ID:
docker ps

Then stop the container:
```bash
docker stop <container_id>
```
---

This `README.md` is designed to be clear, informative, and beginner-friendly. It covers all essential sections, from a quick overview to detailed setup instructions and a usage guide. Make sure to replace `https://github.com/yourusername/rockylinux-apache-docker.git` with your actual GitHub repository URL.

