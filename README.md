# Spring Boot CRUD API

A simple CRUD (Create, Read, Update, Delete) REST API built with Spring Boot and MySQL, managing a `User` entity.

## Features
- Create, retrieve, update, and delete users
- Unique email constraint
- Swagger UI for API documentation (`http://localhost:7788/swagger-ui.html`)

## Endpoints
| Method   | Endpoint                 | Description          |
|----------|--------------------------|----------------------|
| `POST`   | `/user/save`             | Create a new user   |
| `GET`    | `/user/find-by-id/{id}`   | Get user by ID      |
| `GET`    | `/user/find-by-email/{email}` | Get user by email |
| `GET`    | `/user/all`               | Get all users       |
| `DELETE` | `/user/remove/{email}`    | Delete user by email |
| `PATCH`  | `/user/edit/{id}`         | Update user by ID   |

## Setup
1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/your-repo-name.git
   cd your-repo-name
   ```
2. Configure the database in application.yml:
   ```yml
   spring:
   datasource:
     url: jdbc:mysql://yourURL?createDatabaseIfNotExist=true
     username: yourUsername
     password: yourPassword
   ```

3. Run the application:
   ```sh
   mvn spring-boot:run
   ```


