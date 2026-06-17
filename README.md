# Task Tracker

A full-stack Task Tracker application built using Spring Boot and React. The application allows users to create, view, update, and manage task lists through a REST API backend and a modern React frontend.

---

## Features

- Create task lists
- View all task lists
- Update existing task lists
- Delete task lists
- RESTful API architecture
- PostgreSQL database integration
- Responsive React frontend
- Docker support

---

## Tech Stack

### Backend
- Java
- Spring Boot
- Spring Data JPA
- Hibernate
- PostgreSQL
- Maven

### Frontend
- React
- TypeScript
- Vite
- Tailwind CSS

### Tools
- Docker
- Git
- GitHub

---

## Project Structure

```text
task-tracker
│
├── backend
│   ├── src
│   ├── pom.xml
│   └── application.properties
│
├── frontend
│   ├── src
│   ├── public
│   ├── package.json
│   └── vite.config.ts
│
└── README.md
```

---

## Backend Configuration

Update the database settings inside:

```properties
src/main/resources/application.properties
```

Example:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/postgres
spring.datasource.username=postgres
spring.datasource.password=your_password

spring.jpa.hibernate.ddl-auto=update
```

---

## Running PostgreSQL with Docker

Start PostgreSQL container:

```bash
docker compose up -d
```

Verify container is running:

```bash
docker ps
```

---

## Running the Backend

Navigate to backend folder:

```bash
cd backend
```

Run the application:

```bash
mvn spring-boot:run
```

Backend runs on:

```text
http://localhost:8081/api
```

---

## Running the Frontend

Navigate to frontend folder:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Start development server:

```bash
npm run dev
```

Frontend runs on:

```text
http://localhost:5173
```

---

## API Endpoints

Example endpoints:

### Task Lists

```http
GET /api/task-lists
```

```http
POST /api/task-lists
```

```http
PUT /api/task-lists/{id}
```

```http
DELETE /api/task-lists/{id}
```

---

## Screenshots


<img width="1051" height="928" alt="Screenshot 2026-06-17 101442" src="https://github.com/user-attachments/assets/df08f4ab-b8d8-4dcc-bb08-59797ce83cb9" />


```

---

## What I Learned

While building this project I learned:

- Spring Boot fundamentals
- REST API development
- Spring Data JPA
- PostgreSQL integration
- Docker basics
- React and TypeScript integration
- Frontend and backend communication
- Git and GitHub workflow

---

## Future Improvements

- User Authentication
- Spring Security
- JWT Authentication
- Task priorities
- Due dates
- Search and filtering
- Deployment to cloud

---

## Author

Yashodhar G K

GitHub:
https://github.com/yashodhargk7-debug
