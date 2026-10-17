# 📘 Assignment: Building REST APIs with FastAPI

## 🎯 Objective

Build a REST API for managing a small collection of books with FastAPI. Practice defining routes, handling JSON requests, validating input, and returning appropriate HTTP status codes.

## 📝 Tasks

### 🛠️ Create and Run a FastAPI Application

#### Description

Set up a FastAPI application for the book API and run it locally. Use the interactive API documentation to confirm that the application is available.

#### Requirements
Completed program should:

- Install FastAPI and Uvicorn, and define the application in `main.py`.
- Provide a `GET /` endpoint that returns a short confirmation message.
- Start with `uvicorn main:app --reload` and show the interactive documentation at `/docs`.

### 🛠️ Add Book Collection Endpoints

#### Description

Store books in an in-memory collection and add endpoints for listing and creating books. Define a Pydantic model for the data clients must provide.

#### Requirements
Completed program should:

- Define a request model with a book title and author.
- Implement `GET /books` to return all books, including an empty list when none have been added.
- Implement `POST /books` to validate and add a book, assign it a unique integer ID, and return the created book with status `201 Created`.

### 🛠️ Complete Book CRUD Operations

#### Description

Add endpoints to retrieve, replace, and delete an individual book by its ID. Return useful HTTP responses when a requested book does not exist.

#### Requirements
Completed program should:

- Implement `GET /books/{book_id}` to return the matching book.
- Implement `PUT /books/{book_id}` to replace a book's title and author using a validated request body.
- Implement `DELETE /books/{book_id}` to remove the matching book and return status `204 No Content`.
- Return status `404 Not Found` when a requested book ID does not exist.
