# REST API with Go, Gin, JWT, and SQLite3

## Overview

This repository contains a **RESTful API** built using the following technologies:

- **Go**: A statically typed, compiled programming language designed for scalability and efficiency.
- **Gin**: A high-performance HTTP web framework written in Go, perfect for building APIs.
- **JWT (JSON Web Tokens)**: Used for secure user authentication and authorization.
- **SQLite3**: A lightweight, serverless SQL database engine used for data persistence.

## Features

- **User Authentication**: Secure login and registration with JWT tokens.
- **CRUD Operations**: Basic Create, Read, Update, and Delete operations on resources.
- **JWT-Based Authorization**: Protect endpoints using token-based authentication.
- **SQLite3 Integration**: Data is stored in a local SQLite database, allowing for easy management and queries.

## Endpoints

| Method | Endpoint                | Description                        | Auth Required |
|--------|-------------------------|------------------------------------|---------------|
| POST   | `/signup`               | Register a new user                | No            |
| POST   | `/login`                | Authenticate and get JWT token     | No            |
| GET    | `/events`               | Fetch all resources                | No            |
| POST   | `/events`               | Create a new resource              | Yes           |
| GET    | `/events/:id`           | Get a specific resource by ID      | No            |
| PUT    | `/events/:id`           | Update a resource by ID            | Yes           |
| DELETE | `/events/:id`           | Delete a resource by ID            | Yes           |
| POST   | `/events/:id/register`  | Update a resource by ID            | Yes           |
| DELETE | `/events/:id/register`  | Delete a resource by ID            | Yes           |
