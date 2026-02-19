# 📚 Book Manager Application

A simple web application that allows users to manage a list of books. Users can add, view, update, and delete books.

---

## 🛠️ Technologies Used

- **Frontend:** Angular, HTML, CSS, TypeScript
- **Backend:** ASP.NET Core Web API, C#
- **Communication:** RESTful API with HTTP requests

---

## 📋 Features

- ✅ View all books in a table
- ✅ Add a new book
- ✅ Edit an existing book
- ✅ Delete a book
- ✅ In-memory data storage on the backend

---

## 📁 Project Structure

```
Assignment-Enhanzer/
│
├── BookApi/                  # ASP.NET C# Backend
│   ├── Controllers/
│   │   └── BooksController.cs
│   ├── Book.cs
│   ├── Program.cs
│   └── BookApi.csproj
│
└── book-frontend/            # Angular Frontend
    └── src/
        └── app/
            ├── app.ts
            ├── app.html
            ├── app.css
            ├── app.config.ts
            └── book.service.ts
```

---

## ⚙️ Prerequisites

Make sure you have the following installed before running the application:

- [Node.js](https://nodejs.org/) (LTS version)
- [Angular CLI](https://angular.io/cli) (`npm install -g @angular/cli`)
- [.NET 8 SDK](https://dotnet.microsoft.com/en-us/download/dotnet/8.0)
- [VS Code](https://code.visualstudio.com/)

---

## 🚀 How to Run the Application

### Step 1 — Run the Backend (ASP.NET API)

Open a Command Prompt or terminal and navigate to the `BookApi` folder:

```bash
cd BookApi
dotnet run
```

The API will start running at:
```
http://localhost:5000/api/books
```

---

### Step 2 — Run the Frontend (Angular)

Open a Command Prompt or terminal and navigate to the `book-frontend` folder:

```bash
cd book-frontend
ng serve
```

Then open your browser and go to:
```
http://localhost:4200
```

---

## 📡 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/books` | Get all books |
| GET | `/api/books/{id}` | Get a single book |
| POST | `/api/books` | Add a new book |
| PUT | `/api/books/{id}` | Update a book |
| DELETE | `/api/books/{id}` | Delete a book |

---

## 📖 Book Model

| Property | Type | Description |
|----------|------|-------------|
| `id` | int | Unique identifier |
| `title` | string | Title of the book |
| `author` | string | Author of the book |
| `isbn` | string | ISBN number |
| `publicationDate` | string | Publication date |

---

## 📝 Notes

- The backend uses an **in-memory list** to store books. Data will reset when the backend is restarted.
- Make sure **both** the backend and frontend are running at the same time.
- CORS is configured to allow requests from `http://localhost:4200`.

---

## 👨‍💻 Developed By

Developed as part of the **Trainee/Associate Software Engineer Assignment** for **Enhanzer (Pvt) Ltd**.
