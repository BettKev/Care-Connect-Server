# Care-Connect-Server

CareConnect Server is a backend service for managing and tracking Persons with Disabilities (PWD) data. It provides endpoints for registering, updating, and monitoring users via a REST API using json-server.

## Table of Contents

1. Prerequisites
2. Installation
3. Usage
4. API Endpoints
5. Environment Variables
6. Contributing
7. License

## Prerequisites

Before you begin, ensure you have the following installed:

Node.js (version 18.x or later recommended)
Yarn or npm

## Installation

1. Clone the repository:

```
git clone https://github.com/BettKev/Care-Connect-Server.git

cd Care-Connect-Server
```

2. Install dependencies:

```
yarn install
```

If you're using npm:

```
npm install
```

3. Ensure json-server is installed (if not already):

```
yarn add json-server
```

## Usage
1. Start the server:

```
yarn start
```

Or, with npm:

```
npm start
```
2. Access the server: The server will run on https://care-connect-server.onrender.com/ by default.

# API Endpoints

Here are the main API endpoints provided by the server:

## Users

- GET /users – Get all registered users
- GET /users/:id – Get a specific user by ID
- POST /users – Register a new user
- PATCH /users/:id – Update user information
- DELETE /users/:id – Remove a user

Example db.json structure:

```
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
PORT=5000 yarn start
```

Or for npm:

```
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

## License

This project is licensed under the MIT License. See the LICENSE file for details.