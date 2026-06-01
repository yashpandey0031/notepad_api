# Notes API

A CRUD API for a note taking application with history tracking, built with FastAPI and SQLite.

## Getting Started

**Install dependencies**
pip install fastapi uvicorn sqlalchemy

**Run the server**
uvicorn main:app --reload

**Test the endpoints**
Visit http://127.0.0.1:8000/docs or
Visit https://notepad-api-jjgy.onrender.com

## Endpoints

| Method | Endpoint            | Description                                  |
| ------ | ------------------- | -------------------------------------------- |
| POST   | /notes              | Create a new note                            |
| GET    | /notes              | Get all notes                                |
| GET    | /notes/{id}         | Get a single note                            |
| PUT    | /notes/{id}         | Update a note (saves old version to history) |
| DELETE | /notes/{id}         | Delete a note                                |
| GET    | /notes/{id}/history | Get all previous versions of a note          |
| POST   | /login              | Login with a account for accessing anything  |
| POST   | /register           | register with a username and passowrd        |

## Tech Stack

- FastAPI
- SQLite
- SQLAlchemy
- postgresql
- JWT (python-jose)
- Passlib (bcrypt)
- render/neon for deployment
