
---

## 🚀 Tech Stack

| Layer     | Technology                        |
|-----------|-----------------------------------|
| Frontend  | HTML, CSS, JavaScript     |
| Backend   | Spring Boot,  JPA                 |
| Database  | MySQL                             |

---

## 🧑‍💻 Frontend (ZIDIOConnect UI)

### ✨ Features

- Login form with credential validation
- Profile form to update full name, contact, about, and resume file
- Responsive UI with a professional layout
- Smooth section toggling using vanilla JS

### 🛠 How to Run

1. Open `index.html` in your browser.
2. Ensure backend is running at the specified API URL (`http://localhost:8080`).
3. Update `script.js` to POST to `/api/students/login` and `/api/students/{id}` as required.

---

## 🔒 Backend (Spring Boot API)

### 📁 Location

`/Zidio_backend`

### 📦 Key Modules

- `StudentController` – Handles login, register, profile update
- `StudentService` – Core business logic
- `StudentRepository` – JPA interface
- `Student` – JPA entity
- `JWT Security` – Secured login via JSON Web Tokens

### 🔐 API Endpoints

| Method | Endpoint              | Description           |
|--------|-----------------------|-----------------------|
| POST   | `/api/students/login` | Login                 |
| POST   | `/api/students/register`| Register new student |
| PUT    | `/api/students/{id}`  | Update profile        |

### 🛠 How to Run

1. Make sure Java 17+ and Maven are installed.
2. Navigate to the backend project directory:

```bash
cd Zidio_backend

mvn clean install
mvn spring-boot:run
