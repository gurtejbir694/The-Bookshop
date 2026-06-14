# The Bookshop 📚

An end-to-end full-stack e-commerce web application designed and built during my industrial training at **Solitaire Infosys Pvt. Ltd.** The platform leverages Python, Django, and Bootstrap to allow users to securely browse books by categories, study comprehensive author biographies, discover related books, and read or download educational PDFs.

---

## 🛠️ Tech Stack & Architecture

* **Backend Framework:** Python & Django (MTV Architecture)
* **Frontend Design:** HTML5, CSS3, Bootstrap, jQuery, Slick Slider (UI Plugins)
* **Database Management:** SQLite (Pre-seeded dataset included for testing)

---

## 🚀 Architectural Systems Implemented

### Role-Based Access Control (RBAC)

Dedicated portal workflows separating:

* **Admin Accounts**

  * Comprehensive CRUD operations for authors, categories, and books through Django Admin.
* **Authenticated Users**

  * User registration and login.
  * Secure authentication workflows.
  * Communication and contact functionalities.

### Relational Database Design

Structured using One-to-Many relationships:

* Category → Books
* Author → Books

### File Management & PDF Delivery

Configured secure media endpoints to serve and distribute educational PDF resources dynamically through the backend.

---

## 📐 System Mapping

> **Note:** High-level architecture derived from project specifications documented during industrial training.

### Entity-Relationship (E-R) Diagram

```text
       [Categories] (1) --------- Has --------- (M) [Books] (M)
            |                                         |
           (M)                                       (M)
        Writes In                                 Has Written
            |                                         |
            +----------------- (1) [Author] <---------+
```

### Data Flow Diagram (Level-0)

```text
 [ Admin ] ---- CRUD Operations ----> ( The Bookshop Web App ) <---- View & Auth ---- [ User ]
```

---

## ✨ Features

* User Registration & Authentication
* Book Browsing by Category
* Detailed Author Profiles
* Related Book Recommendations
* PDF Reading & Download Support
* Responsive Bootstrap-Based UI
* Admin Dashboard for Content Management
* Secure Media File Handling

---

## 💻 Local Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/gurtejbir694/The-Bookshop.git
cd The-Bookshop
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Apply Database Migrations

```bash
python manage.py migrate
```

### 4. Start the Development Server

```bash
python manage.py runserver
```

### 5. Open in Browser

Visit:

```text
http://127.0.0.1:8000/
```

---

## 📂 Project Structure

```text
The-Bookshop/
│
├── blog/
├── media/
├── clothes/
├── db.sqlite3
├── manage.py
├── requirements.txt
└── README.md
```

---

## 🎯 Learning Outcomes

During the development of this project, I gained practical experience in:

* Django MTV Architecture
* Database Modeling & ORM
* Authentication & Authorization
* CRUD Application Development
* File Handling and Media Management
* Responsive UI Design with Bootstrap
* Full-Stack Web Application Deployment Concepts

---


