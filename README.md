# 📦 Inventory Management System
**Python | Streamlit | SQL**

## 🔍 Project Overview

The **Inventory Management System** is a web-based application that allows users to manage inventory data **without writing any SQL queries**.

This project is designed for real-world users such as **managers, team leads, and operations staff** who need to work with inventory and supplier data but may not have SQL knowledge. The system provides a **simple and interactive interface** to view data, update inventory, place reorders, and track product history.

It simulates how **real business inventory systems** are built by combining a structured SQL backend with a user-friendly Python frontend.

---

## 🏗️ Project Architecture

### User --> ### Streamlit UI (Python) --> ### SQL Database (Tables, Views, Procedures, Functions)


---

## 🧩 Step 1: SQL Database (Backend)

The SQL database stores all inventory data and enforces business rules.

### Database Features
- Tables for core business data
- Views for reports and summaries
- Stored Procedures for actions like receiving stock
- Functions for business logic such as reorder checks

---

## 🗄️ Database Tables

### 1. Products
- Product ID
- Product Name
- Category
- Price
- Stock Quantity
- Reorder Level
- Supplier ID

### 2. Reorder Records
- Supplier ID
- Product ID
- Reorder Quantity
- Reorder Date
- Status (Ordered / Received)

### 3. Shipments
- Shipment ID
- Product ID
- Supplier ID
- Quantity Received
- Shipment Date

### 4. Stock Entries
- Entry ID
- Product ID
- Change Quantity
- Change Type (In / Out)
- Entry Date

### 5. Suppliers
- Supplier ID
- Supplier Name
- Contact Name
- Email
- Phone
- Address

---

## 🔗 Table Relationships

- Suppliers ↔ Products (Supplier ID)
- Suppliers ↔ Shipments (Supplier ID)
- Products ↔ Shipments (Product ID)
- Products ↔ Reorder Records (Product ID)
- Products ↔ Stock Entries (Product ID)

These relationships ensure data accuracy and consistency.

---

## 📊 Key Business Insights

The dashboard displays:
- Total suppliers
- Total products
- Total categories
- Sales value (last 3 months)
- Restock cost (last 3 months)
- Low stock items without pending reorder
- Supplier contact details
- Product stock with supplier information
- Products needing reorder
- Complete product transaction history

All insights are available **without writing SQL queries**.

---

## 🖥️ Step 2: Streamlit Application (Frontend)

The frontend is built using **Python Streamlit** and provides an easy-to-use interface.

### Navigation Sections

#### 1️⃣ Basic Information
Displays:
- Inventory and supplier metrics
- Supplier contact details table
- Product stock and reorder tables

#### 2️⃣ Operational Tasks

**➕ Add New Product**
- Enter product details
- Click *Add Product*
- Product is saved directly to the database

**📜 Product History**
- Select a product
- View shipments, stock changes, and transactions

**🛒 Place Reorder**
- Select product and quantity
- Click *Place Reorder*
- Reorder is stored in the database

**📦 Receive Reorder**
- Select pending reorder
- Click *Mark as Received*
- Stock and shipment records are updated automatically

---

## 🚀 Why This Project Matters

- Combines SQL backend with Python frontend
- Uses real database features (views, procedures, functions)
- Simulates real-world inventory and operations systems
- Designed for non-technical users
- Demonstrates end-to-end application development

---

## 🧠 Skills Gained

- Advanced SQL (Views, Stored Procedures, Functions)
- MySQL and Python integration
- Streamlit dashboard development
- Inventory and operations workflows
- Backend and frontend integration

---

## 📌 Use Cases

- Inventory tracking
- Supplier management
- Stock monitoring
- Sales and restock analysis
- Operations dashboards

---

## 🔮 Future Enhancements

- User authentication
- Role-based access control
- Visual analytics and charts
- Report export (CSV / PDF)

---

## 🙌 Conclusion

This project demonstrates how a real-world inventory management tool can be built using SQL and Python. It focuses on usability, data accuracy, and business logic, making it suitable for both technical and non-technical users.
