# ✅ Todo App Backend – Internship Project

A secure and efficient **Todo List REST API** built with **Node.js**, **Express**, and **MongoDB**, developed as part of my **CodeXIntern Internship**.  
This project demonstrates **JWT authentication**, **user-specific task management**, and a clean **MVC architecture** — making it production-ready and easy to scale.

---

## 📌 Table of Contents

- [🚀 Project Overview](#-project-overview)
- [🛠️ Tech Stack](#️-tech-stack)
- [✨ Features](#-features)
- [📁 Folder Structure](#-folder-structure)
- [🔐 Environment Variables](#-environment-variables)
- [⚙️ Installation & Setup](#️-installation--setup)
- [📬 API Endpoints](#-api-endpoints)
- [📮 Postman Testing](#-postman-testing)
- [👨‍💻 Author](#-author)
- [✅ Final Notes](#-final-notes)

---

## 🚀 Project Overview

The **Todo App Backend** allows users to:

- ✅ Register & log in securely
- ✅ Manage their personal todo list
- ✅ Perform full CRUD operations
- ✅ Access protected endpoints with JWT

This backend is fully functional and built using **real-world standards**.

---

## 🛠️ Tech Stack

| Layer        | Technology              |
|--------------|--------------------------|
| **Runtime**  | Node.js                  |
| **Framework**| Express.js               |
| **Database** | MongoDB with Mongoose    |
| **Auth**     | JSON Web Token (JWT)     |
| **Password Hashing** | bcryptjs        |
| **Validation** | express-validator      |
| **Environment Config** | dotenv         |
| **Testing Tool** | Postman              |

---

## ✨ Features

- 🔐 **JWT-Based Authentication**
- 🧾 **Full CRUD** on Todos
- 👤 **User-specific data isolation**
- 🗂️ **Clean and modular folder structure**
- 📅 **Optional support for due dates and priorities**
- 🧪 **Postman Collection included**

---

## 📁 Folder Structure

todo-backend/
├── config/ # MongoDB connection
├── controllers/ # Route logic for auth and todos
├── middleware/ # Auth middleware
├── models/ # Mongoose models
├── routes/ # API route handlers
├── .env # Environment variables (not pushed)
├── app.js # Express setup
├── server.js # Entry point
├── package.json
└── README.md

---

## 🔐 Environment Variables

Create a `.env` file in the root with:

PORT=5000
MONGO_URI=mongodb://127.0.0.1:27017/todo_db
JWT_SECRET=yourSecretKey

---

## ⚙️ Installation & Setup

```bash
# 1. Clone the repository
git clone https://github.com/Yuvraj-Singh20/todo-backend.git

# 2. Navigate into the folder
cd todo-backend

# 3. Install dependencies
npm install

# 4. Create your .env file
touch .env   # (or manually create)
# Add PORT, MONGO_URI, JWT_SECRET

# 5. Start the development server
nodemon server.js

✅ Server running on: http://localhost:5000
📬 API Endpoints
👤 Auth Routes
Method	Endpoint	Description	Access
POST	/api/users/register	Register new user	Public
POST	/api/users/login	Login user & get JWT	Public

📝 Todo Routes
All routes below require a valid Bearer Token in headers.

Method	Endpoint	Description
POST	/api/todos	Create a new todo
GET	/api/todos	Get all user's todos
PUT	/api/todos/:id	Update specific todo
DELETE	/api/todos/:id	Delete specific todo

📮 Postman Testing
A full Postman collection is included to simplify testing:

📂 todo-backend-postman-collection.json

✅ How to Use
Open Postman
Import the collection file
Register or login a user
Copy the token → go to Authorization tab → Type: Bearer Token → Paste it
Test all todo routes securely


👨‍💻 Author
Yuvraj Singh
Backend Developer Intern @ CodeXIntern


🔗 GitHub – Yuvraj-Singh20
💼 LinkedIn – Yuvraj Singh


✅ Final Notes
This project was built to demonstrate:

✅ Secure user auth with JWT
✅ Best practices in Node.js backend development
✅ Clean and modular architecture
✅ Readiness for full-stack integration

Feel free to fork ⭐, clone 📥, or contribute 👨‍💻
Thanks for checking it out!

📦 Happy Coding!
