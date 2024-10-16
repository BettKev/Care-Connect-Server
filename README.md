# Care-Connect-Server
CareConnect Server is a backend service for managing and tracking Persons with Disabilities (PWD) data. It provides endpoints for registering, updating, and monitoring users via a REST API using json-server.

## Table of Contents
Prerequisites
Installation
Usage
API Endpoints
Environment Variables
Contributing
License

## Prerequisites
Before you begin, ensure you have the following installed:

Node.js (version 18.x or later recommended)
Yarn or npm

## Installation
1. Clone the repository:
```
bash
Copy code
git clone https://github.com/BettKev/Care-Connect-Server.git
cd Care-Connect-Server
```
2. Install dependencies:
```
bash
Copy code
yarn install
```
If you're using npm:
```
bash
Copy code
npm install
```
3. Ensure json-server is installed (if not already):
```
bash
Copy code
yarn add json-server
```
## Usage
1. Start the server:
```
bash
Copy code
yarn start
```
Or, with npm:
```
bash
Copy code
npm start
```
2. Access the server: The server will run on http://localhost:3000 by default.

# API Endpoints
Here are the main API endpoints provided by the server:

## Users
GET /users – Get all registered users
GET /users/:id – Get a specific user by ID
POST /users – Register a new user
PATCH /users/:id – Update user information
DELETE /users/:id – Remove a user

Example db.json structure:
```
json
Copy code
{
  "users": [
    {
      "id": 1,
      "name": "John Doe",
      "disability": "Visual Impairment",
      "status": "Active"
    }
  ]
}
```
## Environment Variables
You can customize the port by setting an environment variable in the terminal before starting the server:
```
bash
Copy code
PORT=5000 yarn start
```
Or for npm:
```
bash
Copy code
PORT=5000 npm start
```
If not set, the server defaults to port 3000.

## Contributing
We welcome contributions! To get started:

1. Fork the repository.
2. Create a new branch (git checkout -b feature-branch).
3. Make your changes and commit them (git commit -m "Add feature").
4. Push to your branch (git push origin feature-branch).
5. Open a pull request.
6. 
## License
This project is licensed under the MIT License. See the LICENSE file for details.