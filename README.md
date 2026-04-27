Flask Dockerized App
A containerized Python Flask web application built and deployed using Docker. Demonstrates real-world containerization practices including multi-stage awareness, dependency isolation, and container portability.

🛠️ Tech Stack

Python 3 — Flask web framework
Docker — containerization and image management
Dockerfile — custom image build with dependency management


📁 Project Structure
flask-docker-app/
├── app.py              # Flask application entry point
├── Dockerfile          # Container build instructions
└── requirements.txt    # Python dependencies

🚀 Getting Started
Prerequisites

Docker installed on your machine

Build the Docker Image
bashdocker build -t flask-docker-app .
Run the Container
bashdocker run -d -p 5000:5000 flask-docker-app
Access the Application
http://localhost:5000

🐳 Dockerfile Overview
The Dockerfile follows container best practices:

Uses an official Python base image
Installs dependencies from requirements.txt before copying app code (layer caching optimization)
Exposes the correct application port
Runs the Flask app as the container entrypoint


💡 Key Concepts Demonstrated

Containerization — packaging a Python app with all its dependencies into a portable Docker image
Layer caching — structuring Dockerfile to maximize build cache efficiency
Port mapping — exposing container ports to the host machine
Dependency isolation — using requirements.txt to manage and freeze Python packages


🔗 Related Projects

terraform-aws-ec2-nginx — Infrastructure as Code with Terraform
docker-aws-ecr-pipeline — Pushing Docker images to AWS ECR


📝 Author
Syed Tahoor Ali Shah

GitHub: @tahoorshah
Medium: @tahoorshah
LinkedIn: syedtahooralishah
