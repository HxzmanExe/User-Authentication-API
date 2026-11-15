
# User Authentication API

A RESTful User Authentication API built using Node.js, Express.js, and MongoDB.

## Technologies Used
- Node.js
- Express.js
- MongoDB Atlas
- Mongoose
- bcryptjs
- JSON Web Token (JWT)
- dotenv
- Postman

## Features
- User registration
- Secure password hashing
- User login
- JWT token generation
- Authentication middleware
- Protected profile route
- Input validation and error handling

## API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| POST | /register | Register a new user |
| POST | /login | Login an existing user |
| GET | /profile | Access protected user profile |

## Setup Instructions

1. Clone this repository.
2. Open the project folder in VS Code.
3. Install dependencies:

   ```bash
   npm install
   ```

4. Create a `.env` file and configure:

   ```env
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_secret_key
   ```

5. Start the server:

   ```bash
   node server.js
   ```

6. Test the API using Postman.

## Testing

The API endpoints were tested using Postman, including successful registration, login, and protected profile access.

## Security

Passwords are hashed using bcryptjs, and JWT tokens are used to protect authenticated routes.
