# 루즈한 (Rujhan Website)

A web application built with Spring Boot and Mustache that provides user management, authentication, and a simple blog/community board system.

## Features

### User Management

* User Registration
* User Login
* Session-based Authentication
* My Page (User Information)

### Blog / Board System

* Create Posts
* View Post List
* Read Individual Posts
* Delete Posts
* Search Posts

### Member Management

* Register Members
* View Member List
* Manage Member Information

### UI

* Responsive design using Bootstrap
* Navigation Menu
* Search Bar
* Alert Messages

---

## Technology Stack

### Backend

* Java
* Spring Boot
* Spring MVC
* Spring Data JPA

### Frontend

* Mustache Template Engine
* HTML5
* CSS3
* Bootstrap 5

### Database

* H2 Database

### Build Tool

* Maven

---

## Project Structure

```text
src
├── main
│   ├── java
│   │   └── com.example.project
│   │       ├── controller
│   │       ├── service
│   │       ├── repository
│   │       ├── entity
│   │       └── dto
│   │
│   └── resources
│       ├── templates
│       ├── static
│       └── application.properties
│
└── test
```

---

## Main Components

### Controller Layer

Handles HTTP requests and page navigation.

Examples:

* MemberController
* LoginController
* ArticleController
* PostController

### Service Layer

Contains business logic.

Examples:

* MemberService
* LoginService
* PostService

### Repository Layer

Responsible for database access using Spring Data JPA.

Examples:

* MemberRepository
* PostRepository

### View Layer

Built using Mustache templates.

Examples:

* home.mustache
* login.mustache
* members.mustache
* posts.mustache

---

## Database

This project uses H2 Database for development.

Example entity:

```java
@Entity
public class Post {

    @Id
    @GeneratedValue
    private Long id;

    private String title;
    private String content;
}
```

---

## How to Run

### Requirements

* Java 17 (or later)
* Maven

### Clone Repository

```bash
git clone https://github.com/yourusername/rujhan-website.git
```

### Run Application

```bash
mvn spring-boot:run
```

or run the main application class directly from your IDE.

### Access Application

```text
http://localhost:8080
```

---

## Screenshots

### Home Page

(Add screenshot here)

### Login Page

(Add screenshot here)

### Blog Page

(Add screenshot here)

### Member Management

(Add screenshot here)

---

## Future Improvements

* Password Encryption using Spring Security
* Post Update Feature
* Comment System
* File Upload
* Kakao Login
* Google OAuth Login
* Pagination
* Role-based Access Control (Admin/User)

---

## Author

Rujhan Munawwaruzzaman

Software Engineering Student

Developed as a Spring Boot learning project focusing on MVC architecture, session authentication, CRUD operations, and template-based web development.
