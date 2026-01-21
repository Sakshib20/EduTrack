# 🎓 EduTrack

**EduTrack** is a backend class management system developed using **Java** and **Spring Boot**. It provides robust RESTful APIs for managing academic batches, utilizing **MongoDB** for efficient NoSQL storage.

The application follows a strict **layered architecture** (Controller-Service-Repository) to ensure separation of concerns and maintainability.

## 🛠️ Tech Stack

* **Language:** Java
* **Framework:** Spring Boot
* **Database:** MongoDB
* **Testing Client:** Postman
* **Build Tool:** Maven

## 🚀 Key Features

* **RESTful API Design:** Standardized endpoints for accessing resources.
* **Layered Architecture:** Clean separation of logic:
  * `Controller`: Handles HTTP requests.
  * `Service`: Contains business logic.
  * `Repository`: Manages database interactions.
* **NoSQL Integration:** Scalable data storage using MongoDB.

## 🔌 API Endpoints

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `GET` | `/batches` | Retrieve all batch entries |
| `POST` | `/batches` | Create a new batch entry |
| `PUT` | `/batches/id/{id}` | Update a batch (Name/Fees) by ID |
| `DELETE` | `/batches/id/{id}` | Delete a batch by ID |

### 📝 Sample Request Body (JSON)
Use this format for **POST** and **PUT** requests:
```json
{
    "name": "PPA",
    "fees": "18000"
}
