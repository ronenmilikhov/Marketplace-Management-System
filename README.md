# Marketplace Management System (.NET / C#)

An Object-Oriented desktop marketplace application developed in C# and Windows Forms. The system models a multi-role retail environment, supporting buyers, sellers, item catalogs, and transactional order workflows with robust domain-level validation.

---

## 🌟 Key Features

* **Multi-Role Domain Modeling:**
  * Clean separation of entities: `User`, `Buyer`, `Seller`, `Item`, and `Address`.
  * Distinct workflows and permissions for sellers and buyers.

* **Inventory & Catalog Management:**
  * Categorized inventory management (Electronics, Clothing, Office, Kids, etc.).
  * Dynamic stock tracking and price calculations.

* **Order Processing & Transactions:**
  * End-to-end purchasing workflow connecting Buyer ↔ Item ↔ Seller.
  * Automatic inventory decrement and transaction logging upon sale execution.

* **Validation & UI/UX:**
  * Multi-step dialog flows for item creation and customer checkout.
  * Comprehensive input validation using regular expressions (Regex) and type checking to ensure data integrity.

* **Data Persistence:**
  * File I/O persistence preserving seller inventories, product catalogs, and transaction logs across sessions.

---

## 🛠️ Architecture & Tech Stack

* **Language:** C#
* **Framework:** .NET Framework
* **UI Framework:** Windows Forms (WinForms)
* **Design Patterns:** Object-Oriented Programming (Encapsulation, Inheritance, Polymorphism)
* **Storage:** File I/O Serialization

---
