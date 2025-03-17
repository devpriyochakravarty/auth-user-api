Authentication and User Management API

A Node.js backend API that provides user authentication with JWT and complete user CRUD operations.

Features

- User Authentication (signup, login, logout)
- JWT-based authentication with refresh tokens
- Complete CRUD API for user management
- Role-based access control (user/admin roles)
- MongoDB integration

Tech Stack

- Node.js
- Express.js
- MongoDB with Mongoose
- JSON Web Tokens (JWT)
- bcryptjs for password hashing

Prerequisites

- Node.js (v14 or above)
- MongoDB installed locally or MongoDB Atlas account

 Installation

1. Clone the repository
git clone <repository-url>
cd auth-user-api


2. Install dependencies
npm install


3. Set up environment variables
Create a .env file in the root directory and add the following:
PORT=3000
MONGODB_URI=mongodb://localhost:27017/auth_user_api
JWT_SECRET=your_jwt_secret_key
JWT_EXPIRE=1d


4. Start the server
npm start


API Endpoints

 Authentication Routes
- POST /api/v1/auth/signup - Register a new user
- POST /api/v1/auth/login - Login a user
- GET /api/v1/auth/logout - Logout a user (requires authentication)
- GET /api/v1/auth/me - Get logged in user info (requires authentication)

 User Management Routes (Admin only)
- GET /api/v1/users - Get all users
- POST /api/v1/users - Create a new
