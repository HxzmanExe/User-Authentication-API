# User Authentication API

A RESTful User Authentication API developed using Node.js, Express.js, and MongoDB. This project provides secure user registration, login, password hashing, and JWT-based authentication.

## Technologies Used

- Node.js
- Express.js
- MongoDB Atlas
- Mongoose
- bcryptjs
- JSON Web Token (JWT)
- dotenv
- Postman
- Git and GitHub

## Features

- User registration
- Secure password hashing using bcryptjs
- User login and credential verification
- JWT token generation
- Authentication middleware
- Protected user profile route
- Input validation and error handling
- MongoDB database integration

## API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| POST | /register | Register a new user |
| POST | /login | Login an existing user |
| GET | /profile | Access protected user profile |

## Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/HxzmanExe/User-Authentication-API.git
```

### 2. Open the project folder

```bash
cd User-Authentication-API
```

### 3. Install dependencies

```bash
npm install
```

### 4. Configure environment variables

Create a `.env` file in the project root and add:

```env
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
```

Replace the example values with your own credentials. Never upload your `.env` file or expose database credentials on GitHub.

### 5. Start the server

```bash
node server.js
```

The server runs at:

`http://localhost:3000`

## Testing

Use Postman to test the API endpoints.

- **Register:** Send a POST request to `/register` with user details.
- **Login:** Send a POST request to `/login` with registered credentials.
- **Profile:** Send a GET request to `/profile` with the JWT token in the Authorization header using Bearer Token authentication.

The API has been tested for successful registration, login, protected profile access, and authentication error responses.

## Security

- Passwords are hashed using bcryptjs before storage.
- JWT tokens are used to authenticate protected routes.
- Unauthorized requests are rejected by authentication middleware.
- Environment variables are used to protect sensitive configuration values.

## GitHub Repository

[User Authentication API – GitHub](https://github.com/HxzmanExe/User-Authentication-API)
