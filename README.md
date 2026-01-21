# 🎓 EduTrack

**EduTrack** is a backend class management system developed using **Java** and **Spring Boot**. It provides robust RESTful APIs for managing academic batches and entries, utilizing **MongoDB** for efficient NoSQL storage.

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
* **Health Checks:** Dedicated endpoints to monitor system status.
* **NoSQL Integration:** Scalable data storage using MongoDB.

## 🔌 API Endpoints

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `GET` | `/journal` | Retrieve all batch entries |
| `POST` | `/journal` | Create a new batch entry |
| `GET` | `/journal/id/{myId}` | Get a specific entry by ID |
| `GET` | `/health-check` | Verify application status |

*(Note: Update the endpoint paths above if they differ in your actual Controller code).*

## ⚙️ Setup & Installation

1.  **Clone the repository**
    ```bash
    git clone [https://github.com/Sakshib20/EduTrack.git](https://github.com/Sakshib20/EduTrack.git)
    ```
2.  **Configure Database**
    Ensure MongoDB is running locally on port `27017`.
3.  **Run the Application**
    ```bash
    ./mvnw spring-boot:run
    ```

---
*Developed by [Sakshi Bhapkar](https://github.com/Sakshib20)*
