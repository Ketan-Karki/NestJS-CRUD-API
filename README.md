# NestJS API Tutorial

This repository contains the code for building a CRUD REST API using NestJS, as demonstrated in the video tutorial by Vladimir.

## Table of Contents
- Introduction
- Prerequisites
- Installation
- Project Structure
- Modules
- Running the Application
- Testing
- Contributing
- License

## Introduction
In this tutorial, we build a scalable and maintainable CRUD REST API using NestJS. The project includes authentication, end-to-end tests, and integration with relational databases using Prisma.

## Prerequisites
- Basic understanding of JavaScript ES6 and TypeScript
- Node.js (version 16 or later)
- NestJS CLI
- Docker (for database setup)

## Installation
1. Clone the repository:
    ```bash
    git clone <repository-url>
    cd nestjs-api-tutorial
    ```

2. Install dependencies:
    ```bash
    yarn install
    ```

3. Install NestJS CLI globally:
    ```bash
    npm install -g @nestjs/cli
    ```

4. Set up the database:
    ```bash
    docker-compose up -d
    ```

## Project Structure
- `src/`: Contains the source code
  - `auth/`: Authentication module
  - `bookmarks/`: Bookmarks module
  - `common/`: Common utilities and services
  - `prisma/`: Prisma schema and migrations
- `test/`: End-to-end tests
- `docker-compose.yml`: Docker configuration for the database

## Modules
### Auth Module
Handles user authentication, including sign-up and login functionalities.

### Bookmarks Module
Manages CRUD operations for bookmarks.

### Prisma Module
Encapsulates database logic and provides a connection to the database.

## Running the Application
1. Start the application in development mode:
    ```bash
    yarn start:dev
    ```

2. The application will run on `http://localhost:3333`.

## Testing
1. Run end-to-end tests:
    ```bash
    yarn test:e2e
    ```

2. Ensure the database is cleaned and restarted before each test run.

## Contributing
Feel free to open issues or submit pull requests. For major changes, please open an issue first to discuss what you would like to change.

## License
This project is licensed under the MIT License.

## Credits
This project follows the tutorial from [NestJs Course for Beginners - Create a REST API](https://www.youtube.com/watch?v=GHTA143_b-s). Special thanks to **Vladimir** for the comprehensive guide.
