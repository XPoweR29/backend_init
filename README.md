# Express TypeScript Starter Project

This repository is a starter template for building backend applications using Express, TypeScript, and common middleware. It serves as a foundation for initializing a new project with basic request handling and structure without configuring a database. 

## Features

- **TypeScript** for type safety and modern JavaScript features.
- **Express** framework for handling HTTP requests and routing.
- **Helmet** for basic security hardening.
- **Centralized Error Handling** for catching and processing errors.
- **Modular Architecture** with a clear separation of concerns using controllers, services, and routers.

## Project Structure

The project is organized in a modular way to ensure easy scalability and maintenance.

```plaintext
backend_init/
├── node_modules/
├── src/
│   ├── db/                  # (To be added) Database configuration (TypeORM)
│   ├── middleware/          # Custom middleware
│   │   └── handleError.ts   # Global error handling middleware
│   ├── modules/             # Feature modules
│   │   ├── greeting/        # Example module
│   │   └── user/            # User module placeholder
│   ├── types/               # Custom types and exceptions
│   │   └── httpExeptions.ts # Example custom exception handling
│   └── utils/               # Utility functions
│       └── serverLog.ts     # Utility for logging server start
├── .env                     # Environment variables
├── .gitignore               # Ignored files and directories
├── nodemon.json             # Nodemon configuration for development
├── package-lock.json        # NPM dependency tree lock file
├── package.json             # Project dependencies and scripts
├── README.md                # Project documentation
└── tsconfig.json            # TypeScript configuration

```

## Getting Started
To get started with this project, follow the steps below:

Prerequisites
Node.js (version 14 or higher recommended)
npm (Node Package Manager) or yarn
Installation
Clone the repository:
```
git clone https://github.com/XPoweR29/backend_init.git
cd backend_init
```

Install dependencies:

```
npm install
# or
yarn install
```

Running the Application
To run the application in development mode, use:

```
npm run dev
# or
yarn dev
```

The server will start at http://localhost:3000 (or the port specified in your .env file).

## Note on Database Configuration
This project currently does not have a configured database. It is recommended to use TypeORM or another ORM for managing database operations. Make sure to initialize the database connection in the src/db/ folder or appropriate module. Follow the official TypeORM documentation for setup instructions.