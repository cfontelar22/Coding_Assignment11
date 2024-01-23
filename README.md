# Fontelar, Christma - Coding Assignment 11

This repository contains a Dockerized React web application for the "Codin 1" website. Follow the instructions below to set up and run the application on your local machine.

## Prerequisites

- Docker installed on your machine. You can download Docker [here](https://www.docker.com/get-started).

## Getting Started

1. **Clone the Repository:**
   git clone https://github.com/cfontelar22/Coding_Assignment11

2. **Build the Docker Image:**

   docker build -t fontelar_christma_coding_assignment11 .

3. **Run the Docker Container**

   docker run -p 7775:7775 fontelar_christma_coding_assignment11

4. **Access the Application**

   Open your web browser and navigate to http://localhost:7775. You should see the "Codin 1" website.

5. **Stopping the Container**
   To stop the running container, use the following command:
   docker stop $(docker ps -q)

6. **Removing the Container**
   To remove the container, use the following command:
   docker rm $(docker ps -a -q)

## Dockerfile Details
The Dockerfile used to build the environment is included in this repository. It creates a development environment that displays an "h1" tag with the text "Codin 1" using Create React App. The container is named "fontelar_christma_coding_assignment11", and the site files are hosted in a workdir called "fontelar_christma_site".
