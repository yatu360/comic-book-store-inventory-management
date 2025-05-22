# 🦸 Comic Book Store Inventory Management System

A RESTful web service for managing comic book inventory, selling comics, viewing sales history, and automated stock replenishment.

---

## 🚀 Features

- 🔍 Search for comics using:
  - Title, issue number, volume
  - Publisher, publication date, cover date
  - Writers, characters, team names
  - Special edition filter
- 🛒 Sell comics (with stock validation)
- 📈 View sale history per comic
- 🔁 Automatically replenish stock based on date
- 🗃️ PostgreSQL for persistent storage

---

## 🧱 Tech Stack

- Java 17+
- Spring Boot
- Spring Data JPA
- PostgreSQL
- Maven
- Lombok
- Flyway (optional)
- Swagger UI (optional)
- **GitHub Actions** (CI for build & test)

---

## ⚙️ Getting Started

### 📁 Clone the project

```bash
git clone https://github.com/your-username/comic-store-inventory.git
cd comic-store-inventory
```
mvn spring-boot:run

GET /api/comics/search

POST /api/comics/{comicId}/sell

GET /api/comics/{comicId}/sales

# Project Structure
src
 └── main
     ├── java/com/example/comicstore
     │    ├── controller
     │    ├── service
     │    ├── repository
     │    ├── model
     │    └── scheduler
     └── resources
          └── application.yml
