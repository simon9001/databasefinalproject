# databasefinalproject
# E-Commerce Store Database (MySQL)

## 📌 Project Objective
The goal of this project is to **design and implement a full-featured relational database** using MySQL for a real-world use case.  
This database models an **E-commerce Store**, handling customers, products, orders, payments, and shipping in a structured and normalized way.

---

## 🏗 Database Schema Overview
The database schema includes the following main entities:

- **Customers** → Stores user details.
- **Addresses** → Each customer can have multiple addresses.
- **Products** → Catalog of items available for purchase.
- **Orders** → Records customer purchases.
- **Order Items** → Connects products and orders (Many-to-Many relationship).
- **Payments** → Stores payment information for each order.
- **Shipping** → Tracks delivery details for each order.

---

## 🔗 Relationships
- **One-to-Many**:
  - Customers → Orders  
  - Customers → Addresses  
  - Orders → Order Items  

- **Many-to-Many**:
  - Orders ↔ Products (via `order_items` table)

- **One-to-One**:
  - Orders → Payments  
  - Orders → Shipping  

---

## 📂 Project Files
- `ecommerce_store.sql` → Contains:
  - `CREATE DATABASE` statement  
  - `CREATE TABLE` statements  
  - Relationship constraints (`PRIMARY KEY`, `FOREIGN KEY`, `UNIQUE`, `NOT NULL`, `CHECK`)  

---
