# 📚 Book Library API

A RESTful API for managing a book library, built with Spring Boot, JPA/Hibernate and PostgreSQL.

## 🚀 Features

* Create books
* Get all books
* Get a book by ID
* Update books
* Delete books
* Store data in PostgreSQL

## 🛠️ Technologies

* Java 21
* Spring Boot
* Spring Web
* Spring Data JPA
* Hibernate
* PostgreSQL
* Maven

## 📁 Project Structure

```text
src/
├── main/
│   ├── java/
│   │   └── com.example.booklibrary/
│   │       ├── controller/
│   │       ├── service/
│   │       ├── repository/
│   │       └── model/
│   │
│   └── resources/
│       └── application.properties/
│
└── test/
```

## 🔌 API Endpoints

| Method | Endpoint          | Description       |
| ------ | ----------------- | ----------------- |
| GET    | `/api/books`      | Get all books     |
| GET    | `/api/books/{id}` | Get a book by ID  |
| POST   | `/api/books`      | Create a new book |
| PUT    | `/api/books/{id}` | Update a book     |
| DELETE | `/api/books/{id}` | Delete a book     |

## 📖 Book

Example request:

```json
{
  "title": "Clean Code",
  "author": "Robert C. Martin",
  "isbn": "9780132350884",
  "publicationYear": 2008,
  "available": true
}
```

## ⚙️ Requirements

Before running the application, make sure you have:

* Java 21
* Maven
* PostgreSQL

## ▶️ Running the Application

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/book-library-api.git
```

Move into the project directory:

```bash
cd book-library-api
```

Configure your PostgreSQL database in `application.properties`.

Then run:

```bash
./mvnw spring-boot:run
```

The API will be available at:

```text
http://localhost:8080
```

## 🧪 Running Tests

Run the test suite with:

```bash
./mvnw test
```

## 📚 What I Learned

This project is a practical exercise to learn and demonstrate:

* Building REST APIs with Spring Boot
* Structuring a Spring Boot application using Controllers, Services and Repositories
* Working with JPA and Hibernate
* Connecting a Spring Boot application to PostgreSQL
* Implementing CRUD operations
* Handling HTTP requests and responses
* Writing tests for a backend application

## 🔮 Future Improvements

* Add request validation
* Add global exception handling
* Introduce DTOs
* Add pagination and filtering
* Improve test coverage
* Add Docker and Docker Compose
* Add API documentation with OpenAPI/Swagger
