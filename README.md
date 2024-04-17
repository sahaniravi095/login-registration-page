
# Login & Registration Page using MAER Stack

This is a login and registration page application built using the MAER stack, which consists of:

- **MongoDB**: The database for storing user data.
- **Angular**: The frontend framework for building the user interface.
- **Express**: The web application framework for building the backend REST API.
- **Redis**: The in-memory data store for caching and session management.

## Table of Contents

- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Configuration](#configuration)
- [Usage](#usage)
- [API Documentation](#api-documentation)
- [Contributing](#contributing)
- [License](#license)

## Features

- User registration and login functionality.
- Secure password storage using hashing.
- Session management with Redis.
- Responsive frontend built with Angular.
- REST API built with Express for handling user authentication and data.
- Validation and error handling for user inputs.

## Prerequisites

Before you begin, ensure you have the following installed:

- [Node.js](https://nodejs.org/) (version 14 or higher)
- [MongoDB](https://www.mongodb.com/) (running locally or on a remote server)
- [Redis](https://redis.io/) (running locally or on a remote server)
- [Angular CLI](https://angular.io/cli) (version 12 or higher)

## Installation

1. Clone the repository:

    ```bash
    git clone <repository-url>
    cd <repository-folder>
    ```

2. Install backend dependencies:

    ```bash
    cd server
    npm install
    ```

3. Install frontend dependencies:

    ```bash
    cd ../frontend
    npm install
    ```

## Configuration

1. Configure the backend:
    ```plaintext
    MONGO_URI=mongodb://localhost:27017/your_database_name
    REDIS_HOST=localhost
    REDIS_PORT=6379
    SESSION_SECRET=your_secret_key
    ```

2. Configure the frontend:

    - In the `frontend` folder, create a file named `environment.ts` for development or `environment.prod.ts` for production.
    - Define the following configuration settings:

    ```typescript
    export const environment = {
      production: false,
      apiUrl: 'http://localhost:3000/api',
    };
    ```

## Usage

1. Start the backend server:

    ```bash
    cd server
    node index.js
    ```

2. Start the frontend application:

    ```bash
    cd ../frontend
    ng serve
    ```

3. Access the application in your web browser at `http://localhost:4200`.

## API Documentation

For the REST API endpoints provided by the backend, you can use tools such as [Postman](https://www.postman.com/) or [Swagger](https://swagger.io/) to interact with and test the API.

## Contributing

Contributions to this project are welcome! Please follow the standard GitHub flow of forking the repository, creating a new branch, and submitting a pull request with your changes.

## License

This project is licensed under the [MIT License](LICENSE). You are free to use, modify, and distribute the code as per the license terms.

---
