# Dicoding Bookshelf API

![Node.js](https://img.shields.io/badge/Node.js-v14.17.0-green) ![Hapi.js](https://img.shields.io/badge/Hapi.js-v20.1.5-blue) ![License](https://img.shields.io/badge/license-MIT-brightgreen)

This project is a simple Bookshelf API built using Node.js and Hapi.js. The API allows users to manage a collection of books by providing endpoints to create, read, update, and delete books. This project is part of the Dicoding "Belajar Membuat Aplikasi Back-End untuk Pemula" course.

---

## Features

- Add a new book
- View all books
- View book details by ID
- Update book information by ID
- Delete a book by ID

---

## Prerequisites

Ensure you have the following installed:

- [Node.js](https://nodejs.org/) (v14.x or later)
- [npm](https://www.npmjs.com/) (v6.x or later)

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yorizpra/dicoding_bookshelf-api.git
   ```

2. Navigate to the project directory:
   ```bash
   cd dicoding_bookshelf-api
   ```

3. Install dependencies:
   ```bash
   npm install
   ```

---

## Running the Application

1. Start the server:
   ```bash
   npm start
   ```

2. The server will run at:
   ```
   http://localhost:5000
   ```

---

## API Endpoints

### 1. Add a Book
- **URL**: `/books`
- **Method**: `POST`
- **Request Body**:
  ```json
  {
    "name": "string",
    "year": "number",
    "author": "string",
    "summary": "string",
    "publisher": "string",
    "pageCount": "number",
    "readPage": "number",
    "reading": "boolean"
  }
  ```
- **Response**:
  - `201 Created`: Book successfully added.

### 2. Get All Books
- **URL**: `/books`
- **Method**: `GET`
- **Response**:
  - `200 OK`: List of all books.

### 3. Get Book Details
- **URL**: `/books/{id}`
- **Method**: `GET`
- **Response**:
  - `200 OK`: Book details.
  - `404 Not Found`: Book ID not found.

### 4. Update a Book
- **URL**: `/books/{id}`
- **Method**: `PUT`
- **Request Body**: Same as Add a Book.
- **Response**:
  - `200 OK`: Book successfully updated.
  - `404 Not Found`: Book ID not found.

### 5. Delete a Book
- **URL**: `/books/{id}`
- **Method**: `DELETE`
- **Response**:
  - `200 OK`: Book successfully deleted.
  - `404 Not Found`: Book ID not found.

---

## Project Structure

```
├── src
│   ├── handler.js        # Request handlers
│   ├── routes.js         # API routes
│   ├── server.js         # Hapi.js server setup
├── package.json          # Project metadata and dependencies
└── README.md             # Project documentation
```

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Acknowledgmentshttps://github.com/yorizpra/dicoding_bookshelf-api

- [Dicoding](https://www.dicoding.com/) for providing the learning platform.
- [Hapi.js](https://hapi.dev/) for the web framework.

---

Feel free to contribute to this project by submitting issues or pull requests!
