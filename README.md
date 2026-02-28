# Bookstore Management Application

![Java](https://img.shields.io/badge/Language-Java-blue)
![JavaFX](https://img.shields.io/badge/Framework-JavaFX-green)
![OOP](https://img.shields.io/badge/Concepts-OOP%20%7C%20State%20Pattern-orange)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow)

A **JavaFX-based bookstore management system** built to demonstrate solid **object-oriented design principles**, **modular architecture**, and the **State Pattern** for dynamic customer rewards.

This project integrates multiple OOP concepts including inheritance, encapsulation, and polymorphism, while showcasing professional JavaFX UI development and design pattern implementation.


---

## 🧭 Overview

The **Bookstore Management Application** simulates a real-world online bookstore that supports two types of users:
- **Admin (Owner)** — manages books and customers.
- **Customer** — browses, purchases, and earns reward points.

The system integrates multiple features, including secure login, cart management, points redemption, and cash checkout.  
It’s built entirely in **Java** using **JavaFX** for the GUI and text file persistence for data storage.

---

## 🎯 Features

### For Customers
- **Login/Logout** using username and password.
- **View Available Books** with title and price.
- **Add/Remove Books from Cart** dynamically.
- **Checkout Options:**
  - Purchase with **cash** (earns points).
  - Redeem **reward points** for discounts or full payments.
- **Automatic Tier Upgrades**:
  - Silver → Gold based on accumulated points.

### For Admin
- **Add or Remove Books** from the system.
- **Manage Users:**
  - Add new customers.
  - Update balances.
  - Remove existing users.
- **Update Inventory** directly via `book.txt` file integration.

---

## 🧩 Design Patterns Used

- **State Pattern** — manages customer reward tiers (`SilverState`, `GoldState`) dynamically based on point thresholds.  
- **Encapsulation & Inheritance** — shared logic in abstract `User` class extended by `Customer` and `Owner`.  
- **Aggregation** — `ShoppingCart` maintains a list of `Book` objects without ownership.  
- **Modular Design** — classes like `Book`, `ShoppingCart`, and `CustomerState` promote scalability and maintainability.

---

## 🧱 Class Structure

| Class | Responsibility |
|-------|----------------|
| `BookStore` | Main application entry point |
| `User` | Abstract class for shared user data and login credentials |
| `Customer` | Handles points, balance, and state transitions |
| `Owner` | Manages books and customers |
| `Book` | Represents book data |
| `ShoppingCart` | Manages added books, total price, and checkout |
| `CustomerState`, `GoldState`, `SilverState` | Implement the State Pattern logic |

Full UML diagrams are included in the `/docs` folder:
- `BookStoreClassDiagram.pdf`
- `UseCaseDiagram.pdf`

---

   ## 📚 Documentation
- [Class Diagram](./docs/BookStoreClassDiagram.pdf)
- [Use Case Diagram](./docs/Use%20Case%20Diagram%20For%20Book%20Store%20App.pdf)

---

## 🗂️ Repository Structure
```
Bookstore-Management-System/
├── src/BookStore/
│   ├── Main.java
│   ├── Customer.java
│   ├── Owner.java
│   ├── Book.java
│   └── ...
├── docs/
│   ├── BookStoreClassDiagram.pdf
│   └── Use Case Diagram For Book Store App.pdf
├── LICENSE
└── README.md
```
---

## 💻 How to Run

1. **Clone this repository**
```bash
git clone https://github.com/ashwin-jakanathan/Bookstore-Management-System.git
cd Bookstore-Management-System
```
2. **Open in your preferred IDE**
- Recommended: IntelliJ IDEA, Eclipse, or VS Code (with the JavaFX plugin installed).

3. **Configure JavaFX (if needed)**
- Ensure you’re using **JDK 17 or newer**.  
- Add the JavaFX library to your project if your IDE doesn’t detect it automatically.  
- In IntelliJ, go to:  
     `File → Project Structure → Libraries → + → JavaFX SDK`

4. **Run the Application**

- Navigate to the file:
     `src/BookStore/Main.java`
- Click Run (in your IDE), or execute this command in the terminal:
```bash
java src/BookStore/Main.java
```
5. **Login Credentials**

- Admin:

  - Username: admin

  - Password: admin

- Customer:

  - Username: customer1

  - Password: 123
