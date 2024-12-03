# Techdome
Devops assignment

Multi-Container Application Deployment 


 Application Overview

This project demonstrates the deployment of a multi-container application with the following components:

•	Frontend: A web application (React/Angular) for the user interface.

•	Backend: A Node.js/Express server that handles API requests and connects to the database.

•	Database: MongoDB for data storage.

The application is deployed using: Docker 
--------------------------------------------------------------------------------------------------------------------------------------
 
Architecture

Components:

1. Frontend:
   Accessible via HTTP on port 80.
   Communicates with the backend for data and operations.

2. Backend:
   Exposed on port 5000.
   Connects to MongoDB for data storage.
   Communicates with the frontend.
3. MongoDB:
   Stores persistent application data.
   Exposed internally on port 27017.

Network:    All services are connected via a shared bridge network (app-network), ensuring isolated communication.

 Deployment Strategies

A. Using Docker Compose

Docker Compose is used for local development. It orchestrates the multi-container setup on a single host.

Steps  followed to Deploy

1. Clone the repositories:

git clone https://github.com/Anand-1432/Techdome-backend.git backend
git clone https://github.com/Anand-1432/Techdome-frontend.git frontend


2. created dockerfile for both frontend and backend
Navigate to the project directory containing the docker-compose.yml file.


3. Build and run the application:

docker-compose up –build

