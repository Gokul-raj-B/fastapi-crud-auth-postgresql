# FastAPI CRUD Application with Authentication

A backend application built using FastAPI and PostgreSQL with JWT-based authentication.

## Features

- User Registration
- User Login
- Password Hashing
- JWT Authentication
- Protected CRUD APIs
- PostgreSQL Database
- SQLAlchemy ORM
- Swagger UI API Documentation

## Technologies Used

- Python
- FastAPI
- PostgreSQL
- SQLAlchemy
- JWT
- Passlib
- Pydantic
- Uvicorn

## API Endpoints

| Method | Endpoint | Description | Authentication |
|--------|----------|-------------|----------------|
| POST | `/register` | Register a new user | No |
| POST | `/login` | Login and get JWT token | No |
| GET | `/users` | Get all users | Yes |
| POST | `/users` | Create a user | Yes |
| PUT | `/users/{user_id}` | Update a user | Yes |
| DELETE | `/users/{user_id}` | Delete a user | Yes |

## Authentication Flow

1. Register a new user using `/register`.
2. Login using `/login`.
3. The API returns a JWT access token.
4. Use the token in Swagger UI using the **Authorize** button.
5. Access the protected CRUD endpoints.

## Run the Project

Install dependencies:

```bash
pip install -r requirements.txt