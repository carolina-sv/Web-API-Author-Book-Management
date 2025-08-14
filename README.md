# 📚 WebAPI - Author & Book Management

A simple yet scalable **.NET 6 Web API** for managing authors and books, designed with a clean architecture pattern.  
It demonstrates the use of **Controllers, Services, Interfaces, Models, and EF Core** for a structured, maintainable backend.

---

## 🚀 Features

- **Author Management**
  - List all authors
  - Search author by ID
- **Book Management** *(extendable)*
- **Layered Architecture** for better maintainability
- **Entity Framework Core** for database access
- **Asynchronous methods** for better performance

---

## 🛠️ Tech Stack

- **.NET 8 Web API**
- **C#**
- **Entity Framework Core**
- **Postgre Database**
- **Dependency Injection**

---

## 📂 Project Structure

WebAPI/
├── Controllers/
│ └── AutorController.cs # API endpoints for authors
│
├── Data/
│ ├── AppDbContext.cs # EF Core DbContext
│ └── Migrations/ # Database migrations
│
├── Models/
│ ├── AutorModel.cs # Author entity
│ ├── LivroModel.cs # Book entity
│ └── ResponseModel.cs # Standard API response wrapper
│
├── Services/
│ └── Autor/
│ ├── AutorInterface.cs # Author service contract
│ └── AutorService.cs # Author service implementation
│
├── Program.cs # API configuration
├── appsettings.json # App configuration
└── WebAPI.http # HTTP test file

---

## ⚙️ API Endpoints

### Author Endpoints

| Method | Route                                   | Description             |
|--------|-----------------------------------------|-------------------------|
| GET    | `/api/Autor/ListarAutores`              | List all authors        |
| GET    | `/api/Autor/BuscarAutorPorId/{idAutor}` | Get author by ID        |

---

## 📦 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/carolina-sv/WebAPI.git
   cd WebAPI

## 🔍 Example Response
{
  "success": true,
  "message": "Author found successfully",
  "data": {
    "id": 1,
    "name": "Jane Austen",
    "books": [
{ "id": 1, "title": "Pride and Prejudice" }
    ]
  }
}

## 🧩 Future Improvements

CRUD for books

Pagination and filtering

Unit tests with xUnit

Authentication & Authorization (JWT)




