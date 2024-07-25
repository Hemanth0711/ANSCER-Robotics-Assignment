# State Management System

## Overview

The State Management System is an application for managing and tracking various states within a system. This application includes features for user authentication, state management, and comprehensive API documentation.

## Features

* User Registration and Login: Secure endpoints for user management.
* State Management: Create, retrieve, and aggregate state data.
* API Documentation: Interactive API documentation using Swagger.
* Testing: Unit tests for verifying API endpoints.

## Prerequisites

Before running the application, ensure you have the following installed:

* Node.js (v14 or higher)
* Docker

## Setup

### Clone the Repository

```bash
git clone <repository-url>
cd state-management-system

Install Dependencies
Bash
npm install

Environment Variables
Create a .env file in the root directory and add the following environment variables:   

Code snippet
PORT=3000
SESSION_SECRET=your-session-secret
MONGO_URI=your-mongodb-uri

Build and Run the Application
Without Docker
Build the application:

Bash
npm run build
Use code with caution.

Start the application:

Bash
npm start

The application will be running on http://localhost:3000.

With Docker
Build the Docker image:

Bash
docker build -t state-management-system .
Use code with caution.

Run the Docker container:

Bash
docker run -p 3000:3000 --env-file .env state-management-system
Use code with caution.

The application will be available at http://localhost:3000.

API Documentation
API documentation is available at http://localhost:3000/api-docs. It is generated using Swagger and provides details about all available endpoints.

Testing
To run unit tests for the API endpoints:

Bash
npm test
Use code with caution.

Postman Collection
A Postman collection for testing the API is provided. Import the State Management API.postman_collection.json file into Postman to use the pre-configured requests.

Notes
For detailed notes and design considerations, refer to the NOTES.md file in the project root.

Troubleshooting
Port Already in Use: Ensure no other service is using port 3000. Change the port in .env if necessary.
