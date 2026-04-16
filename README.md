# 🎓 Online Course Registration System

A web-based application developed using **PHP, MySQL, HTML, CSS, JavaScript, and Bootstrap** that automates the process of course enrollment for students.

## 📌 Project Overview

The **Online Course Registration System** is designed to replace the traditional manual registration process used in educational institutions. It provides a secure and user-friendly platform where students can:

* Log in securely
* View available courses
* Check seat availability in real-time
* Enroll in courses
* View and print enrollment history

---

## 🚀 Features

### 👨‍🎓 Student Module

* Secure login system
* Change password functionality
* View available courses
* Real-time seat availability check (AJAX)
* Course enrollment
* Enrollment history tracking
* Printable enrollment receipt

### 🔐 Security Features

* Password encryption using MD5
* Session management
* IP logging (userlog table)
* Input validation to prevent misuse

---

## 🛠️ Technologies Used

| Category        | Technology                                  |
| --------------- | ------------------------------------------- |
| Frontend        | HTML5, CSS3, Bootstrap, JavaScript (jQuery) |
| Backend         | PHP                                         |
| Database        | MySQL                                       |
| Server          | XAMPP / WAMP                                |
| Version Control | Git & GitHub                                |

---

## 📂 Project Structure

```
online-course-registration/
│
├── index.php                 # Login page
├── dashboard.php            # Student dashboard
├── change-password.php      # Password update
├── check_availability.php   # AJAX seat validation
├── enroll-history.php       # Enrollment records
├── print.php                # Printable receipt
├── logout.php               # Logout system
│
├── includes/
│   ├── config.php           # Database connection
│   └── functions.php        # Helper functions
│
├── assets/
│   ├── css/
│   ├── js/
│   └── images/
│
└── database/
    └── course_registration.sql
```

---

## 🗄️ Database Tables

* **students** → Stores student details and credentials
* **course** → Course details and seat capacity
* **courseenrolls** → Mapping of students to courses
* **userlog** → Login/logout logs with IP tracking

---

## ⚙️ Installation Guide

### Step 1: Clone the Repository

```bash
git clone https://github.com/your-username/online-course-registration.git
```

### Step 2: Move to Server Directory

* Copy project folder to:

  * `htdocs` (XAMPP) OR
  * `www` (WAMP)

### Step 3: Setup Database

1. Open phpMyAdmin
2. Create database: `course_registration`
3. Import `.sql` file from `/database` folder

### Step 4: Configure Database

Edit:

```
includes/config.php
```

Update:

```php
$host = "localhost";
$user = "root";
$password = "";
$dbname = "course_registration";
```

### Step 5: Run Project

Open browser:

```
http://localhost/online-course-registration
```

---

## 🧪 Testing

| Test Case            | Description         | Result              |
| -------------------- | ------------------- | ------------------- |
| Login Validation     | Invalid credentials | Error message shown |
| Duplicate Enrollment | Same course twice   | Blocked             |
| Seat Limit           | Full course         | Disabled            |
| Session Security     | Access after logout | Redirected          |

---

## 📸 Screenshots

*Add your screenshots here (already available in repo)*

---

## 📈 Future Enhancements

* 💳 Payment Gateway Integration
* 📧 Email Notification System
* 🧑‍💼 Admin Dashboard
* 📊 Analytics & Reports

---

## ⚠️ Note

This project uses **MD5 encryption**, which is not recommended for production.
For real-world applications, use:

```
password_hash() and password_verify()
```

---

## 📚 References

* https://www.php.net
* https://getbootstrap.com
* https://www.w3schools.com
* https://dev.mysql.com

---

## 👨‍💻 Author
**Arnav Choudhary **
**Shivam Kedar**
**Rushikesh Khedekar**
**Aayush  Jha**
BCA Final Year Project

---

