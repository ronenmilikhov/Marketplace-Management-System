# Marketplace Management System (.NET / C#)

An object-oriented desktop marketplace application developed in C# with Windows Forms. The application lets users create sellers and buyers, add categorized items to sellers, purchase available items for buyers, and display the current marketplace data.

---

## 🌟 Key Features

* **Domain Modeling:**
  * The domain model contains `User`, `Buyer`, `Seller`, `Item`, and `Address` classes.
  * `Buyer` and `Seller` inherit shared user data from the abstract `User` class.
  * Sellers maintain available items and items sold; the purchase workflow adds selected items to a buyer's current items.

* **Inventory & Catalog Management:**
  * Sellers can add items in the Electronics, Clothing, Office, or Kids categories.
  * Each item has a name, price, category, and generated identifier.
  * A purchase removes the selected item from the seller's available-items list and adds it to the seller's sold-items list.

* **Purchase Workflow:**
  * A buyer is selected first, followed by a seller and one of that seller's available items.
  * The selected item is added to the buyer and marked as sold for the seller.

* **Validation & UI/UX:**
  * Multi-step Windows Forms dialogs guide seller creation, buyer creation, item creation, and purchases.
  * Form event handlers validate required fields, names and addresses with regular expressions, numeric passwords, building numbers, and positive item prices.

* **Data Persistence:**
  * Sellers and their currently available items can be saved to `sellers_data.txt` when using Save and Exit.
  * The file uses manually formatted text records; it is not a general-purpose serialization format.
  * Buyers, buyer current items, buyer purchase history, and detailed sales records are held in memory and are not restored between sessions.

---

## 🛠️ Architecture & Tech Stack

* **Language:** C#
* **Framework:** .NET Framework 4.7.2
* **UI Framework:** Windows Forms (WinForms)
* **Architecture:** Object-oriented domain classes with a Windows Forms UI layer
* **Storage:** Manually formatted text file for seller data

## Application Flow

1. Start the application from `Program.cs`; the main window is `MainForm`.
2. Add sellers, buyers, and items using the corresponding menu actions.
3. Use the buyer purchase workflow to move an available item from a seller to a buyer.
4. Use the display actions to view the current sellers and buyers.
5. Choose Save and Exit to write seller data to `sellers_data.txt`. Closing the window through another route exits without saving.

## Requirements

* Windows
* Visual Studio with .NET Framework 4.7.2 developer tools

---
