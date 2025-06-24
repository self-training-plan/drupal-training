# 🛠️ Week 1: PHP Training Plan (Basic to Advanced with MVC)

## 📍 Overview

This 5-day hands-on training plan is designed to help learners transition from basic PHP and frontend knowledge to building a complete web application using MVC architecture. By the end of the training, learners will create an **Event Manager** app that includes file uploads, role-based access control, and a styled user interface using HTML, CSS, and JavaScript.

---

## 🟦 Day 1: PHP + HTML/CSS Fundamentals

### ✅ Backend (PHP)
- PHP installation and environment setup (XAMPP/LAMP)
- PHP syntax: variables, data types, operators
- Arrays, loops (`for`, `foreach`, `while`)
- Conditional statements (`if`, `else`, `switch`)
- PHP functions and form handling (`$_POST`, `$_GET`)

### 🎨 Frontend (HTML/CSS)
- HTML basics: structure, forms, inputs, semantic tags
- CSS styling: classes, IDs, fonts, colors, box model
- External stylesheets and inline styles

### 🛠️ Hands-On:
- Build a contact form with HTML
- Use PHP to display submitted data
- Style the form using CSS
- Create a PHP-based calculator

---

## 🟦 Day 2: File Upload + JavaScript + OOP Basics

### ✅ Backend (PHP)
- File upload with `$_FILES`, `move_uploaded_file()`
- Server-side validation for file type/size
- Session management: `$_SESSION`, `session_start()`
- OOP Introduction: classes, objects, constructors, `$this`

### 🎨 Frontend (JavaScript + HTML)
- Basic JavaScript for:
  - Form validation
  - Image preview before upload
  - Alerts and confirmation prompts

### 🛠️ Hands-On:
- Profile upload form with JavaScript image preview
- Save uploaded profile picture on the server
- Create a `User` class with login and registration logic
- Use JS to validate file size/type before submission

---

## 🟦 Day 3: Advanced OOP + MySQL + PDO Integration

### ✅ Backend (PHP)
- OOP concepts:
  - Inheritance, abstract classes, interfaces
  - Static methods and class constants
- PDO usage:
  - Secure connection using prepared statements
  - Handling insert, update, delete operations
  - Error handling with `try/catch`

### 🎨 Frontend (HTML/CSS/JS)
- Display data using HTML lists and divs
- Style event listings using CSS Flex/Grid
- Use JavaScript to validate input fields

### 🛠️ Hands-On:
- Create a `UserModel` and `EventModel` using PDO
- Build login system with hashed passwords
- Store and retrieve event data from database
- Display events in a responsive layout (no tables)

---

## 🟦 Day 4: Custom MVC Framework (PHP)

### ✅ Backend (PHP)
- MVC Architecture: Model, View, Controller
- Folder structure setup:
  - `/app/controllers`
  - `/app/models`
  - `/app/views`
  - `/core` for Router, Database, Controller base classes
  - `/public` as web root
- Front Controller pattern (`index.php`)
- Routing using custom `Router` class
- Autoloading classes with Composer (PSR-4)

### 🎨 Frontend (HTML/CSS)
- Header and footer templates
- Reusable layout using `include` or `require`
- Simple navigation UI

### 🛠️ Hands-On:
- Setup working MVC structure
- Create `EventController` with `list()` method
- Create `View` class for rendering views
- Display event list from DB using MVC

---

## 🟦 Day 5: Final Project - Event Manager (Full MVC + RBAC + File Upload)

### ✅ Backend (PHP)
- User authentication (login, logout)
- Role-based access control (`admin`, `user`)
- Event CRUD:
  - Add/Edit/Delete Events
  - Multiple image uploads
- Store uploaded file names in JSON format in DB
- Secure input validation and sanitization
- CSRF token for form security
- Flash messaging using `$_SESSION`

### 🎨 Frontend (HTML/CSS/JS)
- Event form fields:
  - Event Name, Venue, Date, Time
  - Status (Active/Inactive)
  - WYSIWYG Description (CKEditor)
  - Multiple photo uploads
- Use JavaScript to preview selected images
- Layout:
  - Grid/Flexbox based card layout for events
  - Styled buttons, modals for delete confirmation
  - Role-based navigation (Admin/User)

### 🛠️ Final Project Output: Event Manager App

**Admin Capabilities:**
- Login/logout
- Add new event
- Edit existing events
- Delete events
- Upload multiple photos per event
- View all events

**User Capabilities:**
- Login/logout
- View only active events
- View event details

### 🔐 RBAC Implementation:
- Store `role` in `$_SESSION['role']` after login
- Check role in controller before allowing access
- Redirect unauthorized users to error page or home

---

## 🧰 Tools Used

- PHP 8.x
- Apache/Nginx (XAMPP/LAMP)
- MySQL (or MariaDB)
- VS Code or PHPStorm
- Composer for autoloading
- CKEditor (for WYSIWYG)
- Postman (for API simulation/testing)

---

## 📌 Optional Add-ons

- AJAX image upload (for smoother UX)
- Pagination in event listing
- Search and filter by event name/date
- API endpoint for fetching public events (JSON)
- Unit testing using PHPUnit

---

