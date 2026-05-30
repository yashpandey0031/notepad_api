# Notes API

A CRUD API for a note taking application with history tracking, built with FastAPI and SQLite.

## Getting Started

**Install dependencies**
pip install fastapi uvicorn sqlalchemy

**Run the server**
uvicorn main:app --reload

**Test the endpoints**
Visit http://127.0.0.1:8000/docs

## Endpoints

| Method | Endpoint            | Description                                  |
| ------ | ------------------- | -------------------------------------------- |
| POST   | /notes              | Create a new note                            |
| GET    | /notes              | Get all notes                                |
| GET    | /notes/{id}         | Get a single note                            |
| PUT    | /notes/{id}         | Update a note (saves old version to history) |
| DELETE | /notes/{id}         | Delete a note                                |
| GET    | /notes/{id}/history | Get all previous versions of a note          |

## Tech Stack

- FastAPI
- SQLite
- SQLAlchemy
