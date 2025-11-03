# Deploy Docker on Amazon Linux 2 EC2 and Run a Web App

Step-by-step guide to deploying Docker on an Amazon Linux 2 EC2 instance, configuring a web app inside a Docker container. Includes instance setup, security config, Docker installation, and running the web server.

---

## Features

- EC2 instance setup with Amazon Linux 2
- Docker and Docker Compose installation
- Containerized web app deployment
- Security groups for SSH and HTTP
- Easy testing via public IP

---

## Architecture Overview

The project launches an Amazon Linux 2 EC2 instance with Docker installed. A container runs an Apache web server, accessible via the public IP of the EC2. Security groups restrict SSH and HTTP port access, ensuring a secure environment for web hosting inside Docker.

---

## Setup Instructions

1. Launch EC2:
    - Select Amazon Linux 2 AMI, t3.micro for Free Tier.
    - Configure security groups: allow SSH (22), HTTP (80).
    - Assign a key pair.
2. Connect:
    - SSH into the instance: `ssh -i <key.pem> ec2-user@<public-ip>`.
3. Install Docker:
    - Update system and install Docker using the official instructions.
4. Deploy Web App in Docker:
    - Pull or build your Docker image.
    - Run container: `docker run -d -p 80:80 my-web-app`.
5. Test:
    - Visit public IP in your browser.

---

## Connect with me

<p align="center">
  <a href="https://github.com/ShaikhAteeb02">
    <img src="https://img.shields.io/badge/GitHub-Profile-informational?style=for-the-badge&logo=github&logoColor=white&color=181717" alt="GitHub"/>
  </a>
  <a href="https://www.linkedin.com/in/ateeb-ahmed-shaikh-932234192/">
    <img src="https://img.shields.io/badge/LinkedIn-Profile-blue?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
  </a>
</p>
