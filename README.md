# Skygoal Full Stack Task

1. Create authentication apis using express and mongodb as database (login,  signup, userdetails, ect )
2. Create protected routes using auth middleware
3. Use JWT token for all types of authentication for the routes

## Description

The Skygoal Full Stack Task project demonstrates the implementation of authentication APIs using Express and MongoDB. It includes signup, login, user details retrieval, and CRUD operations for users. Protected routes are used to ensure that certain endpoints require authentication using JWT tokens.

## Features

- User authentication (signup, login) with password hashing
- JWT token-based authentication for protected routes
- CRUD operations for managing users (Create, Read, Update, Delete)
- Secure password storage using bcrypt
- Error handling and validation for API requests
- MongoDB database integration with Mongoose ODM

## Installation

1. Clone the repository: `git clone https://github.com/faizan842/Skygoal-Full-Stack-Task`
2. Navigate to the project directory: `cd Skygoal-Full-Stack-Task`
3. Install dependencies: `npm install`
4. Set up environment variables: Create a `.env` file and define the following variables:

- PORT=port_no
- MONGODB_URL=mongodb_url
- JWT_SECRET=jwt_secret

6. Start the server: `npm start`

## Usage

1. Signup: Send a POST request to `/auth/signup` with JSON payload containing `username` and `password`.
2. Login: Send a POST request to `/auth/login` with JSON payload containing `username` and `password`.
3. User details: Access user details by sending a GET request to `/auth/userdetails` with a valid JWT token in the `Authorization` header.
4. CRUD operations for users: Use protected routes (`/users`) for CRUD operations on users. Ensure to include a valid JWT token in the `Authorization` header for authentication.

## API Endpoints

- `POST /auth/signup`: Create a new user
- `POST /auth/login`: Authenticate user and generate JWT token
- `GET /auth/userdetails`: Retrieve user details
- `POST /users`: Create a new user
- `GET /users`: Retrieve all users
- `GET /users/:id`: Retrieve user by ID
- `PUT /users/:id`: Update user by ID
- `DELETE /users/:id`: Delete user by ID

## Technologies Used

- Node.js
- Express.js
- MongoDB
- Mongoose
- JSON Web Tokens (JWT)
- bcrypt
