# 🍽️ foodHub

> A full-stack food ordering web application with role-based access for customers and admins.

![Status](https://img.shields.io/badge/status-in%20development-yellow)
![Frontend](https://img.shields.io/badge/frontend-HTML%20%7C%20CSS%20%7C%20JavaScript-orange)
![Database](https://img.shields.io/badge/database-MySQL-blue)
![License](https://img.shields.io/badge/license-MIT-green)

---

## 📖 About

**foodHub** is a full-stack food ordering web application inspired by platforms like FoodPanda. Customers can browse restaurants and menus, place orders, and track their order status — while admins have a dedicated dashboard to manage menu items, orders, and users. Built as a portfolio project to demonstrate full-stack web development skills with role-based authentication using vanilla HTML, CSS, and JavaScript on the frontend, a Node.js REST API on the backend, and MySQL as the database.

---

## ✨ Features

### 👤 Customer
- 📝 Register and log in securely
- 🍔 Browse available food items and menus
- 🛒 Add items to cart and place orders
- 📦 Track order status in real time
- 📜 View order history

### 🛠️ Admin
- 🔐 Separate admin login and dashboard
- 🍽️ Add, edit, and delete menu items
- 📋 View and manage all incoming orders
- 👥 Manage customer accounts
- 📊 Overview of sales and orders

### General
- 🔑 Role-based authentication (Customer / Admin)
- 📱 Responsive design for mobile and desktop

---

## 🛠️ Tech Stack

| Layer       | Technology                          |
|-------------|-------------------------------------|
| Frontend    | HTML5, CSS3, JavaScript (Vanilla)   |
| Backend     | Node.js + Express                   |
| Database    | MySQL                               |
| Dev Tools   | phpMyAdmin *(optional, for DB GUI)* |

---

## 📁 Project Structure

```
foodHub/
├── frontend/
│   ├── index.html          # Landing / login page
│   ├── customer/           # Customer-facing pages
│   │   ├── menu.html
│   │   ├── cart.html
│   │   └── orders.html
│   ├── admin/              # Admin dashboard pages
│   │   ├── dashboard.html
│   │   ├── menu-manage.html
│   │   └── orders-manage.html
│   ├── css/
│   │   └── styles.css
│   └── js/
│       └── main.js
├── backend/
│   ├── routes/
│   │   ├── auth.js
│   │   ├── menu.js
│   │   └── orders.js
│   ├── controllers/
│   ├── middleware/
│   │   └── authMiddleware.js
│   └── config/
│       └── db.js
├── database/
│   └── foodhub_schema.sql
├── .env.example
├── .gitignore
├── LICENSE
└── README.md
```

---

## 🚀 Getting Started

### Prerequisites

- A web browser
- [Node.js](https://nodejs.org/) (v18 or higher)
- MySQL installed locally (or via XAMPP/WAMP/MAMP)
- *(Optional)* phpMyAdmin for database management

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/codeAFK/food-hub.git
   cd food-hub
   ```

2. **Set up the database**
   - Open MySQL or phpMyAdmin
   - Create a new database called `foodhub`
   - Import the schema:
     ```bash
     mysql -u root -p foodhub < database/foodhub_schema.sql
     ```

3. **Configure the backend**
   - Navigate to `backend/config/`
   - Copy the example env file and fill in your credentials:
     ```bash
     cp .env.example .env
     ```
   - Edit `.env` with your MySQL credentials

4. **Install dependencies and run**
   ```bash
   cd backend
   npm install
   node server.js
   ```

---

## 🗺️ Roadmap

- [x] Project setup and repo initialization
- [ ] Database schema design
- [ ] Backend API — Authentication & role-based access
- [ ] Backend API — Menu management (CRUD)
- [ ] Backend API — Order management
- [ ] Frontend — Landing & login page
- [ ] Frontend — Customer: menu browsing & cart
- [ ] Frontend — Customer: order tracking & history
- [ ] Frontend — Admin: dashboard & menu management
- [ ] Frontend — Admin: order management
- [ ] Deployment

---

## 🤝 Contributing

This is a personal portfolio project, but feedback and suggestions are always welcome! Feel free to open an issue or fork the repo.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 👤 Author

**Your Name**
- GitHub: [@codeAFK](https://github.com/codeAFK)
- Portfolio: 
- LinkedIn:
