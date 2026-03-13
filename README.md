# 🎓 Student Registration Form  
### Python GUI + MySQL Database Project

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![Tkinter](https://img.shields.io/badge/GUI-Tkinter-green)
![Database](https://img.shields.io/badge/Database-MySQL-orange)
![Status](https://img.shields.io/badge/Project-Working-success)

---

# 📌 Project Overview

The **Student Registration Form** is a desktop application developed using **Python Tkinter GUI** and **MySQL database**.

This application allows users to:

✔ Register student details  
✔ Store data in a MySQL database  
✔ Validate input fields  
✔ Display success or error messages  

The system provides a **simple graphical interface for collecting student information**.

---

# 🖼 Application Interface

```
+----------------------------------+
|        REGISTER FORM             |
|----------------------------------|
| Name      : [______________]     |
| Email     : [______________]     |
| Phone     : [______________]     |
| Password  : [______________]     |
|                                  |
|        [   REGISTER   ]          |
+----------------------------------+
```

---

# ⚙ Technologies Used

| Technology | Purpose |
|-------------|--------|
| 🐍 **Python** | Core programming language |
| 🖥 **Tkinter** | GUI interface |
| 🗄 **MySQL** | Database storage |
| 🔌 **mysql-connector-python** | Python–MySQL connection |

---

# 📊 System Workflow

Below is the **data flow of the system**:

```
User Input
   │
   ▼
GUI Form (Tkinter)
   │
   ▼
Input Validation
   │
   ▼
Python Backend Logic
   │
   ▼
MySQL Database
   │
   ▼
Success / Error Message
```

---

# 📈 System Architecture

```
+-------------------+
|      USER         |
+-------------------+
          │
          ▼
+-------------------+
|   Tkinter GUI     |
| Registration Form |
+-------------------+
          │
          ▼
+-------------------+
|  Python Backend   |
|  Validation + SQL |
+-------------------+
          │
          ▼
+-------------------+
|   MySQL Database  |
|   Student Table   |
+-------------------+
```

---

# 🗂 Database Structure

Database Name:

```
registerform
```

Table Name:

```
students
```

Table Schema:

| Field | Type |
|------|------|
| id | INT (Primary Key) |
| name | VARCHAR |
| email | VARCHAR |
| phone | VARCHAR |
| password | VARCHAR |

SQL Command to Create Table:

```sql
CREATE DATABASE registerform;

USE registerform;

CREATE TABLE students (
id INT AUTO_INCREMENT PRIMARY KEY,
name VARCHAR(100),
email VARCHAR(100),
phone VARCHAR(15),
password VARCHAR(100)
);
```

---

# 🚀 Installation Guide

### 1️⃣ Install Required Library

```bash
pip install mysql-connector-python
```

---

### 2️⃣ Start MySQL Server

Use one of the following:

- **XAMPP**
- **MySQL Workbench**
- **Local MySQL Server**

---

### 3️⃣ Configure Database

Update the connection credentials:

```python
host="localhost"
user="root"
password=""
database="registerform"
```

---

### 4️⃣ Run the Program

```bash
python registerform.py
```

---

# 🔑 Key Features

✨ **User-Friendly Interface**  
✨ **Data Validation**  
✨ **Secure Database Storage**  
✨ **Error Handling with Message Boxes**  
✨ **Automatic Field Clearing After Submission**

---

# 🧠 Program Logic

The application follows this process:

1️⃣ User enters details in the GUI form  
2️⃣ Python checks if fields are empty  
3️⃣ If valid → data sent to MySQL  
4️⃣ MySQL stores the student information  
5️⃣ User receives **success confirmation**

---

# 📊 Example Data Flow Graph

```
Entries Submitted
      │
      ▼
Field Validation
      │
      ▼
Database Insert Query
      │
      ▼
Student Record Stored
```

---

# 🔮 Future Improvements

Possible enhancements:

✔ Login authentication system  
✔ Password encryption  
✔ Email verification  
✔ Student dashboard  
✔ Web-based version using Flask  

---

# 👩‍💻 Author

**Amandeep Kaur**  
B.Tech Electronics & Communication Engineering  

💡 Interested in **AI/ML, Python, and Software Development**

---

# ⭐ Support

If you like this project:

⭐ Star the repository  
🍴 Fork the project  
📢 Share with others
