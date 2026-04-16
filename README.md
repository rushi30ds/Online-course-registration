# 🎓 Online Course Registration System

A web-based application developed using **PHP, MySQL, HTML, CSS, JavaScript, and Bootstrap** that automates the course enrollment process for students.

---

## 📌 Project Overview

The **Online Course Registration System** is designed to replace the traditional manual registration system used in educational institutions. It provides a secure and user-friendly platform where students can:

* Log in securely
* View available courses
* Check seat availability in real-time
* Enroll in courses
* View and print enrollment history

This system improves efficiency, reduces manual errors, and ensures proper course management.

---

## 🚀 Features

### 👨‍🎓 Student Module

* Secure login system
* Change password functionality
* View available courses
* Real-time seat availability (AJAX-based)
* Course enrollment
* Enrollment history tracking
* Printable enrollment receipt

### 🛠️ Admin Module

* Manage courses (Add / Edit / Delete)
* Manage students
* View enrollment reports
* Track user activity logs

### 🔐 Security Features

* Password encryption using MD5
* Session management
* IP logging (userlog table)
* Input validation

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
├── admin/                     # Admin panel
├── assets/                    # CSS, JS, images
├── includes/                  # Config & reusable components
├── studentphoto/              # Student images
├── SQL File/                  # Database file
│
├── index.php                  # Login page
├── check_availability.php     # Seat validation
├── enroll-history.php         # Enrollment records
├── print.php                  # Receipt printing
├── logout.php                 # Logout
```

---

## 🗄️ Database Tables

* **students** → Student details and credentials
* **course** → Course details and seat limits
* **courseenrolls** → Student-course mapping
* **userlog** → Login/logout logs

---

## ⚙️ Installation Guide

### 1️⃣ Clone Repository

```bash
git clone https://github.com/rushi30ds/Online-course-registration.git
```

### 2️⃣ Move Project

Copy project folder to:

```
C:\xampp\htdocs\
```

### 3️⃣ Setup Database

* Open **phpMyAdmin**
* Create database: `course_registration`
* Import SQL file from `SQL File/onlinecourse.sql`

### 4️⃣ Configure Database

Edit:

```
includes/config.php
```

```php
$host = "localhost";
$user = "root";
$password = "";
$dbname = "course_registration";
```

### 5️⃣ Run Project

Open browser:

```
http://localhost/online-course
```

---

## 🧪 Testing

| Test Case            | Description   | Result      |
| -------------------- | ------------- | ----------- |
| Login Validation     | Invalid login | Error shown |
| Duplicate Enrollment | Same course   | Blocked     |
| Seat Limit           | No seats      | Disabled    |
| Session Security     | After logout  | Redirected  |

---

## 📸 Screenshots

Screenshots are available in the `/screens` folder.

---

## 📈 Future Enhancements

* 💳 Payment Gateway Integration
* 📧 Email Notification System
* 🧑‍💼 Advanced Admin Dashboard
* 📊 Reports & Analytics

---

## ⚠️ Note

This project uses **MD5 encryption**, which is outdated.
For production systems, use:

```php
password_hash()
password_verify()
```

---

