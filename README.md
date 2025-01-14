# Docker-Project

# Docker Express Application

A simple containerized Express.js application that serves a welcome message.

## Technologies Used
- Node.js
- Express.js
- Docker
- Alpine Linux

## Prerequisites
- Docker installed on your machine
- Node.js (for local development)

## Getting Started

## Deployment
Windows (using WSL)

1. Install prerequisites:

Install WSL2 via PowerShell as administrator:
```
wsl --install
```
- Install Docker Desktop for Windows
-  Ensure WSL2 integration is enabled in Docker Desktop settings

2. Setup project in WSL:
```
# Open WSL terminal and navigate to where you want to clone the project
cd /your/preferred/directory

# Clone the repository
git clone https://github.com/jayB133/Docker-Project.git
cd Docker-Project

# Build the Docker image
docker build -t my-app:1.0 .

# Run container
docker run -d -p 3000:3000 my-app:1.0
```
3. Access the application:

Open http://localhost:3000 in your Windows browser
Or use curl http://localhost:3000 from WSL terminal


Linux Environment

Linux Environment

1. Install prerequisites:
```
# Install Docker
sudo apt-get update
sudo apt-get install docker.io

# Start Docker service
sudo systemctl start docker
sudo systemctl enable docker
```
2. Deploy Applicaiton
```
# Navigate to project directory
cd /path/to/your/project

# Build and run
sudo docker build -t my-app .
sudo docker run -p 3000:3000 my-app
```
3. Access the applicaiton:
```
curl http://localhost:3000
```
