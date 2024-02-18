

# User Management Web API

This project is a simple ASP.NET Core Web API for managing user data.

## Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Technologies Used](#technologies-used)
4. [Getting Started](#getting-started)
5. [API Endpoints](#api-endpoints)
6. [Adding Migrations](#adding-migrations)
7. [Contributing](#contributing)
8. [License](#license)

## Introduction

The User Management Web API provides basic CRUD (Create, Read, Update, Delete) operations for managing user data. It allows clients to interact with user resources via HTTP requests.

## Features

- Create a new user
- Retrieve a list of users
- Retrieve a single user by ID
- Update an existing user
- Delete a user

## Technologies Used

- ASP.NET Core 8.0
- Entity Framework Core
- Microsoft SQL Server (for database storage)

## Getting Started

To run the project locally, follow these steps:

1. Clone this repository to your local machine.
2. Open the solution in Visual Studio.
3. Ensure that you have a local instance of Microsoft SQL Server installed and running.
4. Update the connection string in the `appsettings.json` file to point to your SQL Server instance.
5. Open the Package Manager Console and run the following commands to add migrations and update the database:
   ```
   dotnet ef migrations add InitialCreate
   dotnet ef database update
   ```
6. Build and run the project in Visual Studio.

## API Endpoints

The following API endpoints are available:

- `GET /api/user`: Retrieve a list of all users.
- `GET /api/user/{id}`: Retrieve a single user by ID.
- `POST /api/user`: Create a new user.
- `PUT /api/user/{id}`: Update an existing user.
- `DELETE /api/user/{id}`: Delete a user by ID.

For detailed information about request and response formats, refer to the Swagger documentation provided by the API.

