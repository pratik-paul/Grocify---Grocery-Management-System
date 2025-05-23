# 🛒 Grocify – Grocery Management System

Grocify is a robust and efficient desktop-based Grocery Management System developed using **Python**, **Tkinter**, and **MySQL**. It is designed to simplify inventory tracking, sales management, and customer transactions for grocery store owners and managers.

---

## 🚀 Features

- 📦 Product, Category & Sub-category Management
- 👥 Customer & Employee Record System
- 🧾 Automated Billing and Invoice Generation
- 🔐 Admin Authentication System
- 📊 Real-time Stock Updates
- 🖥️ Tkinter-based Graphical User Interface

---

## ⚙️ Installation & Setup

1. Create the database manually in MySQL:
   ```sql
   CREATE DATABASE grocify;
2. Ensure the following Python modules are installed:
tkinter
pillow

3. Update database credentials in the code (host, user, password) — 23 connector points must be updated.
   
4. Add admin credentials manually via MySQL:
   CREATE TABLE admin (
  id INT PRIMARY KEY,
  username VARCHAR(20),
  password VARCHAR(50)
);
INSERT INTO admin VALUES (1, 'admin', 'admin123');


🗃️ Tables Created Automatically on First Run
admin

customers

employees

invoices

products

⚠️ Notes
Do not use spaces in product or sub-category names — use underscores _ or hyphens -.

Product/category data must be manually synced between code and database for initial setup.

Add hardcoded items at line 1538 of the source code if needed.

💻 Requirements
Python 3.12+

MySQL (local setup)

Windows environment (for Tkinter GUI compatibility)

📄 License
This project is licensed under the MIT License.
