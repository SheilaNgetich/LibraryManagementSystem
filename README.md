# 📚 Java Library Management App 🌸

## ✨ Description

This Library Management System allows admins to manage books and staff in a cozy, user-friendly interface. It features a login system, a charming dashboard, and full CRUD functionality for books and staff — all wrapped in Comic Sans MS and soft purple tones. 🎀📖

## 💫 Features

🔐 Secure Admin Login (username + password from database)

📋 Add / Update Books — Avoid duplicates by updating copies if the same book exists

🧾 Add / Remove Staff — Manage your team with ease

📚 View Books & Staff — Tables show all records neatly

🎯 One Editable Admin — Keep things simple and secure

🏠 Dashboard — All options available after login in one beautiful page

## 🖼️ Screenshots

![Dashboard](https://github.com/SheilaNgetich/LibraryManagementSystem/blob/main/Dashboard.png)

![StaffWindow](https://github.com/SheilaNgetich/LibraryManagementSystem/blob/main/AddStaff.png)

![EditAdmin](https://github.com/SheilaNgetich/LibraryManagementSystem/blob/main/EditAdmin.png)

![RemoveBook](https://github.com/SheilaNgetich/LibraryManagementSystem/blob/main/RemoveBook.png)

![BooksAvailable](https://github.com/SheilaNgetich/LibraryManagementSystem/blob/main/BooksAvailable.png)




## 🛠️ Tech Stack

- **Java Swing** (for GUI)  
- **JDBC + MySQL** (for database interaction)  
- **NetBeans IDE** (for development)  
- Comic Sans MS font for a playful vibe 🌸

---

## ⚙️ How to Run
1. 💾 Clone the repository:

```bash
git clone https://github.com/SheilaNgetich/LibraryManagementSystem.git
```
2. 🧰 Open the project in NetBeans or your favorite Java IDE.

3. 🗃️ Ensure you have MySQL running and create a database with the following tables:
🔐 Sample MySQL Tables
```bash
CREATE DATABASE library_database;
USE library_database;

CREATE TABLE admin (
    user_id INT(50),
    name VARCHAR(50),
    password VARCHAR(50),
    contact VARCHAR(50)
);
-- Sample Admin
INSERT INTO admin VALUES ('admin', 'admin123');

CREATE TABLE books (
    book_id INT PRIMARY KEY,
    category VARCHAR(50),
    name VARCHAR(100),
    author VARCHAR(50),
    copies INT
);

CREATE TABLE staff (
    staff_id INT PRIMARY KEY,
    name VARCHAR(100),
    contact VARCHAR(50)
);
```
## 🪄 How Adding Books Works

📚 When you add a book:

- If the book **already exists** (same name, author, and category), it updates the number of copies.

- It inserts it fresh into the database if it's a **new book**.

✨ Helpful, efficient, and cute — just like you want your app to be!

## 📌 Notes
- Currently uses plain-text passwords — consider hashing for production use!

- Only one admin exists and is editable.

- You can customize the Dashboard and UI as much as you like. 🌸

## 💖 Author
Developed with love by **Sheila** 💻🌷
Feel free to ⭐ the repo or share your version if you like it!
