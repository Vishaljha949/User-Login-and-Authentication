# User Login & Registration App

A simple yet comprehensive user authentication system built with Node.js and MongoDB. This app demonstrates user registration, login, and session management using modern web technologies.

## Features

- User registration with email and password
- User login with email and password
- Password hashing for secure storage
- User session management
- Simple REST API endpoints for authentication

## Technologies Used

- **Node.js**: JavaScript runtime for building server-side applications
- **Express.js**: Web application framework for Node.js
- **MongoDB**: NoSQL database for storing user data
- **Mongoose**: ODM (Object Data Modeling) library for MongoDB
- **bcryptjs**: Library for hashing passwords
- **jsonwebtoken**: Library for generating and verifying JSON Web Tokens (JWTs)
- **dotenv**: Module for loading environment variables

## Installation

1. **Clone the repository:**

    ```bash
    git clone https://github.com/yourusername/user-login-register-app.git
    cd user-login-register-app
    ```

2. **Install dependencies:**

    ```bash
    npm install
    ```

3. **Set up environment variables:**

    Create a `.env` file in the root directory and add your MongoDB connection string and a secret key for JWT:

    ```
    MONGO_URI=your_mongodb_connection_string
    JWT_SECRET=your_jwt_secret_key
    ```

4. **Run the application:**

    ```bash
    npm start
    ```

## API Endpoints

### Register

- **POST** `/api/register`
- **Description**: Registers a new user
- **Request Body**:
    ```json
    {
      "email": "user@example.com",
      "password": "your_password"
    }
    ```

### Login

- **POST** `/api/login`
- **Description**: Authenticates a user and returns a JWT
- **Request Body**:
    ```json
    {
      "email": "user@example.com",
      "password": "your_password"
    }
    ```

## Testing

For testing purposes, you can use tools like Postman or curl to interact with the API endpoints. Ensure that the server is running before making requests.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributing

Feel free to fork the repository and submit pull requests. Contributions are welcome!

