# Spring Boot Person CRUD API with Dozer Mapper
[![Powered by @sotobotero](https://img.shields.io/badge/Powered%20by-%40sotobotero-blue?style=flat-square&logo=twitter)](https://twitter.com/sotobotero)
[![Sotobotero.com](https://img.shields.io/badge/Powered%20by-sotobotero.com-blue?style=flat-square&logo=twitter)](https://sotobotero.com/)

🌟 **Contribuye y Mejora este Proyecto**
¡Este proyecto está en constante evolución y cualquier mejora es bienvenida! 🎉 Si encuentras algo que se pueda optimizar, tienes una idea o quieres corregir errores, no dudes en participar.
### 📌¿Quieres enviar cambios y no sabes cómo?📌
Consulta el paso a paso [**Cómo contribuir con un proyecto en github**](https://github.com/sotobotero/CodeHub/blob/develop/README.md#-cómo-contribuir) para español or [**How to Contribute with github project**](https://github.com/sotobotero/CodeHub/blob/develop/README.md#-how-to-contribute) for English.

## Descripción
This project is a REST API example built with Spring Boot that demonstrates CRUD operations for managing person data. The application uses Dozer Mapper to efficiently map between domain objects and DTOs, maintaining a clean architecture.
## Features
- Complete CRUD operations for person data
- REST API with best practices implementation
- Object mapping with Dozer Mapper
- Clean, scalable architecture for Spring Boot learners
## Requirements
- Java 8+
- Maven

## Setup
1. Clone the repository:
  ```bash
  git clone https://github.com/sotobotero/spring_boot.git
  ```
2. Navigate to the project directory:
  ```bash
  cd spring_boot
  ```
3. Build and run the application:
  ```bash
  mvn clean install
  mvn spring-boot:run
  ```
## API Usage
### Endpoints
- `GET /person` - Retrieve all persons
  ```bash
  curl -X GET http://localhost:8080/person
  ```
- `GET /person/{id}` - Retrieve a specific person
  ```bash
  curl -X GET http://localhost:8080/person/{id}
  ```

- `POST /person` - Create a new person
  ```bash
  curl -X POST http://localhost:8080/person -H "Content-Type: application/json" -d '{
    "firstName": "John",
    "lastName": "Doe",
    "email": "john.doe@example.com"
  }'
  ```

- `PUT /person/{id}` - Update an existing person
  ```bash
  curl -X PUT http://localhost:8080/person/{id} -H "Content-Type: application/json" -d '{
    "firstName": "John",
    "lastName": "Doe",
    "email": "john.doe@example.com"
  }'
  ```

- `DELETE /person/{id}` - Delete a person
  ```bash
  curl -X DELETE http://localhost:8080/person/{id}
  ```

### Request Example

#### POST /person
```json
{
  "firstName": "John",
  "lastName": "Doe",
  "email": "john.doe@example.com"
}
```
