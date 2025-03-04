# Docker_114

A simple Django web application containerized using Docker. This project demonstrates how to set up a basic Django app and run it inside a Docker container using a **Dockerfile** and **Docker Compose**.

## Project Setup

This project includes a basic Django application that returns "Hello, World!" as a response on the main page. It uses Docker to containerize the application, making it easy to run the project on any system with Docker installed.

### Prerequisites

- Docker
- Docker Compose (optional but recommended)

### Steps to Run the Project

1. **Clone the repository**:
   git clone https://github.com/anageguchadze/Docker_114.git
   cd Docker_114

2. Build the Docker image:
    docker build -t my-django-app .
    Run the Docker container:

    docker run -p 8000:8000 my-django-app

Alternatively, if you're using Docker Compose:
    docker-compose up

Access the application: Open a browser and visit http://localhost:8000/, you should see "Hello, World!" displayed.

Files in the Project
    Dockerfile: Defines the steps to build the Docker image for the Django app.
    docker-compose.yml: (Optional) Provides an easy way to manage multi-container Docker applications.
    requirements.txt: Lists the necessary Python dependencies (e.g., Django).
    myproject/: Contains the basic Django project with views and URL configuration.

License
    This project is licensed under the MIT License - see the LICENSE file for details.