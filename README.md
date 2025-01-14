# Docker-Proj2

# Docker Express Application

A simple containerized Express.js application that serves a welcome message.

## Technologies Used
- Node.js
- Express.js
- Docker
- Alpine Linux

## Project Structure
my-app/
├── src/
│   └── server.js    # Express application entry point
├── Dockerfile       # Docker container configuration
├── package.json     # Node.js dependencies and project metadata
└── README.md       # Project documentation


## Prerequisites
- Docker installed on your machine
- Node.js (for local development)

## Getting Started

### Running with Docker

1. Build the Docker image:
```bash
docker build -t my-app . 
```
2. Run the Container:
```bash
docker run -p 3000:3000 my-app
```
