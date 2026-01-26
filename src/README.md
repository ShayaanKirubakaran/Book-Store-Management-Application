# Bookstore Management System

A robust and user-friendly Java application designed to streamline bookstore operations, featuring role-based access for customers and owners, comprehensive inventory management, secure payment processing, and an intuitive graphical interface.

## 🚀 Features

### Customer Features
- **User Registration & Authentication**: Secure login system with role-based access
- **Book Browsing**: Browse and search through the complete book catalog
- **Shopping Cart**: Add, remove, and manage items in the shopping cart
- **Purchase History**: Track previous purchases and order details
- **Customer Loyalty Program**: Silver and Gold membership states with benefits

### Owner Features
- **Inventory Management**: Add, update, and remove books from the catalog
- **User Management**: Manage customer accounts and permissions
- **Sales Analytics**: Monitor sales performance and customer data
- **System Administration**: Full control over bookstore operations

### Core Functionality
- **Database Integration**: Persistent data storage for books, users, and transactions
- **Input Validation**: Robust validation for all user inputs
- **Price Formatting**: Consistent currency formatting throughout the application
- **Scene Management**: Smooth navigation between different application views

## 🛠️ Technologies Used

- **Java**: Core programming language
- **JavaFX**: GUI framework for creating the user interface
- **JDBC**: Database connectivity
- **Object-Oriented Design**: Modular architecture with handlers, models, and state patterns

## 📋 Prerequisites

- Java Development Kit (JDK) 8 or higher
- JavaFX SDK (if not included in JDK)

## 🔧 Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/bookstore-management-system.git
   cd bookstore-management-system
   ```

2. **Compile the application:**
   ```bash
   javac -cp "path/to/javafx/lib/*" src/BookStore/*.java src/BookStore/*/*.java
   ```

3. **Run the application:**
   ```bash
   java -cp "src;path/to/javafx/lib/*" BookStore.BookStoreApplication
   ```

   *Note: Replace `path/to/javafx/lib/*` with the actual path to your JavaFX library files.*

## 📖 Usage

1. **Launch the application** using the run command above
2. **Login** as a customer or owner using provided credentials
3. **Customers** can browse books, add to cart, and make purchases
4. **Owners** can manage inventory and user accounts through the admin interface

### Sample User Credentials
- **Customer**: Username: `customer1`, Password: `pass123`
- **Owner**: Username: `owner1`, Password: `admin123`

## 🏗️ Project Structure

```
BookStore/
├── BookStoreApplication.java    # Main application entry point
├── database/
│   └── DatabaseManager.java     # Database operations
├── handlers/
│   ├── CustomerHandler.java     # Customer operations
│   ├── LoginHandler.java        # Authentication
│   ├── LogoutHandler.java       # Session management
│   ├── OwnerHandler.java        # Owner operations
│   ├── PaymentHandler.java      # Payment processing
│   └── ShoppingCartHandler.java # Cart management
├── models/
│   ├── Book.java                # Book entity
│   ├── Customer.java            # Customer entity
│   ├── Owner.java               # Owner entity
│   ├── ShoppingCart.java        # Shopping cart
│   └── User.java                # Base user class
├── resources/
│   ├── Books.txt                # Book data
│   └── Users.txt                # User data
├── scenes/
│   ├── CustomerCostScene.java   # Customer purchase view
│   ├── CustomerScene.java       # Customer dashboard
│   ├── LoginScene.java          # Login interface
│   ├── OwnerBookManageScene.java # Book management
│   ├── OwnerScene.java          # Owner dashboard
│   ├── OwnerUserManageScene.java # User management
│   ├── SceneManager.java        # Scene navigation
│   └── ShoppingCartScene.java   # Shopping cart view
├── state/
│   ├── CustomerState.java       # Base state
│   ├── GoldState.java           # Gold membership
│   └── SilverState.java         # Silver membership
└── utils/
    ├── InputValidator.java      # Input validation
    └── PriceFormatter.java      # Price formatting
```

## 🎯 Design Patterns

- **State Pattern**: Implemented for customer membership levels (Silver/Gold)
- **Handler Pattern**: Separated business logic into dedicated handler classes
- **MVC Architecture**: Models, views (scenes), and controllers (handlers)

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📞 Contact

- **Project Link**: [https://github.com/yourusername/bookstore-management-system](https://github.com/yourusername/bookstore-management-system)
- **Email**: your.email@example.com

---

*Built with ❤️ using Java and JavaFX*