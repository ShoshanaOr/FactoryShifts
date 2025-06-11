
# 🏭 Factory Management System – Node.js + Express + MongoDB

A full-featured **Web Application** designed for managing employees, departments, and work shifts in a factory environment. This project showcases strong **backend development** using **Node.js**, **Express**, **MongoDB**, and **JWT-based authentication**, with client-side interaction built using **HTML** and native JavaScript.

## 📐 Architecture & Technologies

This project was designed with a layered architecture:
- **Business Logic Layer** (Services)
- **Data Layer** (MongoDB, Mongoose Models)
- **Presentation Layer** (HTML & JS)
- **Security Layer** (express-jwt, login limitations)

> ⚙️ The server was built with **Node.js + Express**, following **RESTful** principles (CRUD operations).
>  
> 🗃️ The database is managed via **MongoDB**, with schema modeling using **Mongoose**.
>  
> 🔐 All routes are protected via **JWT-based authentication**, allowing only authorized users to access the system.

---

## 👤 User Authentication & Authorization

- **JWT Login system** via `https://jsonplaceholder.typicode.com/users` for user validation.
- Each user has a **daily action limit** – once exceeded, the user is **automatically logged out**.
- Actions are logged in a JSON file for auditing.

---

## 🧱 Data Structure Overview

### 🧑 Employees
- First Name / Last Name
- Start Work Year
- Belongs to a Department
- Registered to multiple shifts

### 🏢 Departments
- Department Name
- Managed by an Employee
- Contains multiple Employees

### 🕐 Shifts
- Date
- Start and End Hours
- One or more Employees per shift

### 👥 Users
- Full Name
- Max Actions Allowed
- Daily Action Count

---

## 📄 Pages & Features

### 🔐 Login Page
- Only registered users can log in
- Validates against external API
- Full name appears on all pages
- Log-out option available at all times

### 👥 Employees Page
- Table with employee details and shift history
- Filter employees by department
- Add / Edit / Delete employees
- Assign employees to existing shifts

### 🏢 Departments Page
- List departments with managers and employee names
- Add / Edit / Delete departments
- Reassign employees between departments

### 🕒 Shifts Page
- Create new shifts
- Edit existing shifts
- Assign employees to shifts
- Note: **Shifts cannot be deleted**

### 🔧 Users Page
- View all users
- See remaining actions per day
- No editing or deletion permitted

---

## 🧪 Development Highlights

- 🔄 **REST API** implementation with full CRUD operations
- 🔐 **Role-based access control** using JWT
- 📊 **Data filtering**, user limits, and system security
- 🧠 **Pre-planned architecture** with clean code separation
- 💾 Developed and tested with **Visual Studio Code**

---

## 🚀 Getting Started

1. Clone the repository  
2. Install dependencies  
   ```bash
   npm install
