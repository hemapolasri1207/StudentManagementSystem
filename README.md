# 🎓 Student Management System

## 📌 Overview

This is a full-stack **Student Management System** built using **Node.js, Express.js, MySQL, HTML, CSS, and JavaScript**.
It allows users to perform complete CRUD operations on student data.

---

## 🚀 Features

* ➕ Add new student
* 📋 View all students
* ✏️ Update student details
* ❌ Delete student
* 🔍 Search students by name/email
* 🔃 Sort students (alphabetically)
* ✅ Basic form validation

---

## 🛠️ Tech Stack

**Frontend:**

* HTML
* CSS
* JavaScript

**Backend:**

* Node.js
* Express.js

**Database:**

* MySQL

---

## ⚙️ Setup Instructions

### 1️⃣ Clone the repository

```bash
git clone <your-repo-link>
cd student-management
```

### 2️⃣ Install dependencies

```bash
npm install
```

### 3️⃣ Configure Database

Create a MySQL database:

```sql
CREATE DATABASE student_db;
```

Create table:

```sql
CREATE TABLE students1 (
  id INT AUTO_INCREMENT PRIMARY KEY,
  name VARCHAR(100),
  email VARCHAR(100) UNIQUE,
  course VARCHAR(100),
  created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
```

### 4️⃣ Update DB credentials

In `app.js`:

```js
const db = mysql.createConnection({
  host: "localhost",
  user: "root",
  password: "your_password",
  database: "student_db"
});
```

---

### 5️⃣ Run the server

```bash
node app.js
```

Server will run on:

```
http://localhost:5000
```

---

### 6️⃣ Open Frontend

Open `index.html` in browser.

---

## 🔗 API Endpoints

| Method | Endpoint          | Description      |
| ------ | ----------------- | ---------------- |
| POST   | /api/students     | Add student      |
| GET    | /api/students     | Get all students |
| PUT    | /api/students/:id | Update student   |
| DELETE | /api/students/:id | Delete student   |

---

## 📸 Output

* Displays student list in table
* Supports edit and delete actions
* Dynamic UI updates

---

## 📌 Conclusion

This project demonstrates full-stack development with proper API integration, database handling, and frontend interaction. It fulfills all core requirements of CRUD operations and basic system design.

---

## 👨‍💻 Author

Hema polasri

