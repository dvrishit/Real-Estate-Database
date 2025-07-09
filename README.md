# Real-Estate-Database
# 🏢 Real Estate Management System (REMS)

A comprehensive database-backed system to manage properties, tenants, leases, payments, maintenance, and more.

Developed by:
- **Dangeti Venkata Rishit** (23CSB0A09)
- **Ketha Sriharsha** (23CSB0F21)

---

## 📌 Overview

The **Real Estate Management System (REMS)** is a centralized solution designed to automate and manage real estate operations including:
- Property ownership and leasing
- Tenant lifecycle management
- Financial tracking and payments
- Maintenance and vendor coordination
- Document handling and reporting

This system benefits owners, managers, and tenants by ensuring operational efficiency, transparency, and data accuracy.

---

## 🧩 Key Components

- **Property Management**: Track all property details including size, type, ownership, features, etc.
- **Owners & Managers**: Multiple properties per owner; each managed by a licensed property manager.
- **Tenant Management**: Store tenant information, lease applications, and credit score.
- **Lease Handling**: Manage lease agreements, rent tracking, deposits, and durations.
- **Payment Processing**: Record rent payments and link to leases.
- **Maintenance**: Track requests raised by tenants and assign them to vendors.
- **Utilities & Insurance**: Manage electricity, water, internet, and insurance for each property.
- **Documents**: Store and retrieve contracts, inspection reports, receipts, etc.

---

## 🛠️ Problem Statement

Manual handling of real estate operations leads to:
- Scattered data and inefficiencies
- Communication delays between stakeholders
- Increased chances of errors and delays in decision-making

The proposed system eliminates these problems by using a normalized relational database schema.

---

## 🧱 ER Diagram & Relational Model

The system is designed around 20+ normalized entities such as:

- `PROPERTY`, `OWNER`, `TENANT`, `LEASE`, `PAYMENT`
- `MAINTENANCE_REQUEST`, `VENDOR`, `APPLICATION`
- `UTILITY`, `INSURANCE`, `DOCUMENT`, `EXPENSE`, etc.

Each relation includes appropriate **primary keys**, **foreign keys**, **constraints**, and **check conditions** to ensure data consistency.

---

## 🗄️ Schema and Table Design

Sample table creation syntax:

```sql
CREATE TABLE OWNER (
  OwnerID INT PRIMARY KEY AUTO_INCREMENT,
  Name VARCHAR(100) NOT NULL,
  ContactNumber VARCHAR(15),
  Email VARCHAR(100) UNIQUE
);
```
