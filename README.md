# NestJS Boilerplate with PostgreSQL

A robust and scalable boilerplate for building RESTful APIs using NestJS and PostgreSQL. This starter template incorporates essential features and follows best practices to help kickstart your project with clean, maintainable code.

## Features

- **NestJS**: A progressive Node.js framework for building efficient and reliable server-side applications.
- **PostgreSQL**: Powerful, open-source object-relational database.
- **TypeORM**: Easy-to-use ORM for managing database operations.
- **Authentication**: JWT-based authentication and authorization.
- **Configuration Management**: Environment-based configuration support.
- **Modular Architecture**: Clean and scalable project structure.
- **Error Handling**: Centralized exception handling.
- **Validation**: Request data validation using `class-validator`.

## Prerequisites

- [Node.js](https://nodejs.org/) (v16 or later)
- [PostgreSQL](https://www.postgresql.org/) (v12 or later)
- [npm](https://www.npmjs.com/)

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/oshoup521/nestjs-boilerplate-postgres.git
cd nestjs-boilerplate-postgres
```

### 2. Install Dependencies

Using npm:
```bash
npm install
```

### 3. Set Up Environment Variables

Create a `.env` file in the root of the project and define the required variables. Example:

```env
DATABASE_HOST=localhost
DATABASE_PORT=5432
DATABASE_USER=postgres
DATABASE_PASSWORD=yourpassword
DATABASE_NAME=yourdatabase
JWT_SECRET=your_jwt_secret
PORT=3000
```

### 4. Run the Application

To start the development server:

```bash
npm run start:dev
```

The server will be running at `http://localhost:3000`.

### 5. Run Database Migrations

```bash
npm run typeorm migration:run
```

## Project Structure

```plaintext
src/
├── app.module.ts        # Root module
├── main.ts              # Application entry point
├── auth/                # Authentication module
├── common/              # Shared utilities, interceptors, and guards
├── config/              # Configuration management
├── database/            # Database module and TypeORM entities
└── users/               # Example feature module (Users)
```

## Scripts

- `start`: Start the application in production mode
- `start:dev`: Start the application in development mode
- `start:debug`: Start the application in debug mode
- `build`: Build the application
- `lint`: Run linting checks
- `test`: Run unit tests

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
