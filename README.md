State Management System
Overview
The State Management System is an application for managing and tracking various states within a system. This application includes features for user authentication, state management, and comprehensive API documentation.

Features
User Registration and Login: Secure endpoints for user management.
State Management: Create, retrieve, and aggregate state data.
API Documentation: Interactive API documentation using Swagger.
Testing: Unit tests for verifying API endpoints.
Prerequisites
Before running the application, ensure you have the following installed:

Node.js (v14 or higher)
Docker
Setup
Clone the Repository
bash
Copy code
git clone <repository-url>
cd state-management-system
Install Dependencies
bash
Copy code
npm install
Environment Variables
Create a .env file in the root directory and add the following environment variables:

env
Copy code
PORT=3000
SESSION_SECRET=your-session-secret
MONGO_URI=your-mongodb-uri
Replace your-session-secret with a secure session secret and your-mongodb-uri with your MongoDB connection string.

Build and Run the Application
Without Docker
To build and run the application locally:

Build the application:

bash
Copy code
npm run build
Start the application:

bash
Copy code
npm start
The application will be running on http://localhost:3000.

With Docker
To build and run the application using Docker:

Build the Docker image:

bash
Copy code
docker build -t state-management-system .
Run the Docker container:

bash
Copy code
docker run -p 3000:3000 --env-file .env state-management-system
The application will be available at http://localhost:3000.

API Documentation
API documentation is available at http://localhost:3000/api-docs. It is generated using Swagger and provides details about all available endpoints.

Testing
To run unit tests for the API endpoints:

bash
Copy code
npm test
Postman Collection
A Postman collection for testing the API is provided. Import the State Management API.postman_collection.json file into Postman to use the pre-configured requests.

Notes
For detailed notes and design considerations, refer to the NOTES.md file in the project root.

Troubleshooting
Port Already in Use: Ensure no other service is using port 3000. Change the port in .env if necessary.
Docker Daemon Issues: Ensure Docker is running properly and check Docker's documentation for resolving daemon issues.
