# IN3101 - Enterprise Application Development: Lab Sheet 02
## Building a REST API with Spring Boot

- **Student Name:** E.K.N.H. Wijesinghe  
- **Index Number:** 234237U  
- **Faculty:** Faculty of Information Technology, University of Moratuwa  

---

### Project Overview
This repository contains the complete implementation of **IN3101 Lab Sheet 02 - Building a REST API with Spring Boot**. The application provides full CRUD functionality for a library book management system and OpenAPI / Swagger UI interactive documentation.

### Features
- **Layers:** Entity (JPA), Repository (Spring Data JPA), Service, REST Controller
- **Validation:** Bean Validation constraints (`@NotBlank`, `@PositiveOrZero`)
- **Documentation:** Interactive OpenAPI / Swagger UI documentation with `@Tag`, `@Operation`, and `@ApiResponse`
- **Database:** Configured for MySQL database (`library_db`)

### REST Endpoints
| Method | URL | Description | Expected Status |
|--------|-----|-------------|-----------------|
| `GET` | `/api/books` | Retrieve list of all books | 200 OK |
| `GET` | `/api/books/{id}` | Retrieve single book by ID | 200 OK (404 if missing) |
| `POST` | `/api/books` | Create a new book | 201 Created |
| `PUT` | `/api/books/{id}` | Update an existing book | 200 OK (404 if missing) |
| `DELETE` | `/api/books/{id}` | Delete a book by ID | 204 No Content |

### API Documentation (Swagger UI)
When the application is running, open your browser and navigate to:
- **Swagger UI:** `http://localhost:8080/swagger-ui/index.html`
- **OpenAPI JSON Docs:** `http://localhost:8080/v3/api-docs`
