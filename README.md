# Node.js CI/CD Pipeline with GitHub Actions

This project demonstrates a complete CI/CD pipeline that automatically builds and pushes a Docker image for a Node.js application using GitHub Actions.

## Project Objective

The objective of this project is to automate the process of building and deploying a Node.js application using a CI/CD pipeline.

The pipeline performs the following tasks:

- Automatically triggers on code push
- Installs Node.js dependencies
- Builds a Docker image
- Pushes the image to Docker Hub

This helps streamline the development workflow and ensures consistent builds and deployments.

## Technologies Used

- Node.js
- Docker
- GitHub
- GitHub Actions
- Docker Hub

## Project Structure
nodejs-devops-cicd
│
├── app.js
├── package.json
├── Dockerfile
├── README.md
└── .github
└── workflows
└── main.yml

## CI/CD Pipeline Workflow

The CI/CD pipeline is defined in:
.github/workflows/main.yml


### Pipeline Process

1. Developer pushes code to GitHub repository
2. GitHub Actions pipeline is triggered
3. Node.js dependencies are installed
4. Docker image is built
5. Docker image is pushed to Docker Hub

Pipeline flow:
Code Push → GitHub
↓
GitHub Actions Triggered
↓
Install Dependencies
↓
Build Docker Image
↓
Push Image to Docker Hub

## Docker Image

The Docker image is available at:
prozpek/nodejs-devops-cicd:latest

Docker Pull Command:

docker pull prozpek/nodejs-devops-cicd:latest

Run the container locally:

docker run -p 3000:3000 prozpek/nodejs-devops-cicd

Then open in browser:

http://localhost:3000

## GitHub Actions Workflow

The workflow automatically runs on push to the main branch.

Example workflow steps:

- Checkout repository
- Setup Node.js environment
- Install dependencies
- Build Docker image
- Login to Docker Hub
- Push Docker image

## Learning Outcomes

By completing this project, the following DevOps concepts were implemented:
- CI/CD pipeline automation
- Docker containerization
- Automated image building
- Secure authentication using GitHub Secrets
- Continuous deployment to Docker Hub

## Author

Rajiv
DevOps Intern
