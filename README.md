# 🎓 EduTrack: System Architecture

**EduTrack** is an **integrated backend system** developed using **Java** and **Spring Boot**. It provides robust RESTful APIs for **orchestrating** academic data workflows, utilizing **MongoDB** for high-performance NoSQL data engineering.

The application follows a strict **layered architecture** (Controller-Service-Repository) to ensure modular system integration and maintainability.

## 🛠️ Tech Stack

* **Language:** Java
* **Framework:** Spring Boot
* **Data Integration:** MongoDB (NoSQL)
* **Testing Client:** Postman
* **Build Tool:** Maven

## 🚀 Key Features

* **RESTful Service Orchestration:** Standardized endpoints for seamless system communication.
* **Layered Architecture:** Clean separation of system logic:
  * `Controller`: Manages request routing.
  * `Service`: Handles business logic integration.
  * `Repository`: Manages data persistence layers.
* **NoSQL Data Engineering:** Scalable data management using MongoDB.

## 🔌 System Endpoints

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `GET` | `/batches` | Synchronize and retrieve all records |
| `POST` | `/batches` | Initialize a new system entry |
| `PUT` | `/batches/id/{id}` | Update record states by ID |
| `DELETE` | `/batches/id/{id}` | Terminate a record by ID |

### 📝 Sample Request Body (JSON)
```json
{
    "name": "PPA",
    "fees": "18000"
}