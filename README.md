# 🏨 Hotel Management System

A Java-based desktop application designed to simplify hotel administrative operations through an interactive graphical user interface. The system provides dedicated modules for managing hotel rooms, guest information, and employee records, with file-based data storage and CRUD functionalities.

## 📌 Project Overview

The **Hotel Management System** is developed using Java and Java Swing to provide a centralized platform for handling essential hotel management activities.

The application features an administrator login system and an interactive dashboard that allows administrators to navigate between different management modules. It supports adding, viewing, searching, updating, and deleting records for hotel rooms, guests, and employees.

The project follows Object-Oriented Programming (OOP) principles to maintain a modular and organized codebase. Java file handling is used to store and retrieve application data without requiring an external database management system.

## ✨ Key Features

### 🔐 Administrator Authentication
- Dedicated administrator login interface.
- Username and password verification.
- Access to the centralized management dashboard.

### 🛏️ Room Management
- Add and manage hotel room information.
- Assign unique room IDs.
- Select room categories:
  - Normal
  - VIP
  - VVIP
  - President
- Manage room availability status.
- Set room prices per night.
- Search rooms using their IDs.
- Update and delete room records.

### 👥 Guest Management
- Register new hotel guests.
- Store guest information, including name, age, contact number, and customer ID.
- Record the total duration of a guest's stay.
- Calculate total accommodation costs based on the stay duration.
- Search guest records.
- Update and delete guest information.

### 👨‍💼 Employee Management
- Add new employee records.
- Store employee details, including name, age, contact number, employee ID, and salary.
- View employee information in a tabular format.
- Search employee records.
- Update and delete employee information.

### 📂 File-Based Data Management
- Store customer, employee, and room information in separate text files.
- Retrieve previously stored records.
- Implement CRUD operations using Java file handling.
- Maintain data between application sessions.

### 🖥️ Graphical User Interface
- Interactive desktop interface developed using Java Swing.
- Dedicated login screen and management dashboard.
- Separate interfaces for room, guest, and employee management.
- Data presentation using JTable.
- User interaction through buttons, text fields, combo boxes, and dialog messages.

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| Java | Core application development |
| Java Swing | Graphical User Interface |
| Java AWT | GUI components and event handling |
| Java File Handling | Data persistence and file operations |
| Object-Oriented Programming | Modular application design |

## 🏗️ Project Architecture

The application is organized into separate packages to maintain code readability and separation of responsibilities.

```text
Hotel Management System/
│
├── Start.java
│
├── GUI/
│   ├── Login.java
│   ├── Dashboard.java
│   ├── RoomManagerFrame.java
│   ├── EmployeeManagerFrame.java
│   └── CustomerManagerFrame.java
│
├── Entity/
│   ├── Person.java
│   ├── Customer.java
│   ├── Employee.java
│   └── Room.java
│
├── db/
│   ├── dbConfig/
│   │   └── DbConfig.java
│   ├── customer-log.txt
│   ├── employee-log.txt
│   └── room-log.txt
│
└── Resources/
    ├── dashboard.jpg
    ├── employee.jpg
    ├── guest.png
    ├── login.png
    ├── room.jpg
    └── room-1.jpg
```

### Package Description

**1. GUI**

Contains the application's graphical interfaces and user interaction logic.

- `Login.java` – Administrator authentication.
- `Dashboard.java` – Main navigation dashboard.
- `RoomManagerFrame.java` – Room management interface.
- `EmployeeManagerFrame.java` – Employee management interface.
- `CustomerManagerFrame.java` – Guest management interface.

**2. Entity**

Contains the data models used throughout the application.

- `Person.java` – Abstract parent class containing common personal information.
- `Customer.java` – Represents hotel guest information and accommodation details.
- `Employee.java` – Represents employee information and salary details.
- `Room.java` – Represents hotel room information and availability.

**3. db/dbConfig**

Contains `DbConfig.java`, which handles data storage and retrieval through Java file handling.

**4. Resources**

Contains image assets used throughout the graphical user interface.

## 🧩 Object-Oriented Programming Concepts

The project demonstrates practical implementation of several OOP concepts:

- **Abstraction:** The `Person` class is implemented as an abstract class.
- **Inheritance:** `Customer` and `Employee` inherit common attributes and methods from `Person`.
- **Encapsulation:** Entity attributes are declared private and accessed through getter and setter methods.
- **Polymorphism:** Inheritance and method overriding are used within the entity classes.
- **Constructors:** Parameterized and default constructors are used to initialize objects.

## ⚙️ Data Management and CRUD Operations

The application implements Create, Read, Update, and Delete operations through the `DbConfig.java` class.

| Operation | Description |
|---|---|
| Create | Adds new customer, employee, and room records. |
| Read | Retrieves individual records and lists of stored records. |
| Update | Modifies existing records using their respective IDs. |
| Delete | Removes records from the corresponding storage files. |

### Data Storage Structure

The application uses three separate text files:

- `customer-log.txt` – Stores guest information.
- `employee-log.txt` – Stores employee information.
- `room-log.txt` – Stores hotel room information.

No external database is required for the current implementation.

## 🚀 Getting Started

### Prerequisites

Before running the application, ensure you have:

- Java Development Kit (JDK) installed.
- A Java-compatible IDE such as IntelliJ IDEA, Eclipse, or VS Code.
- Git installed (optional, for cloning the repository).

### Installation

**1. Clone the repository**

```bash
git clone https://github.com/Sazzadul-Haque-Chowdhury/hotel-management-system.git
```

**2. Navigate to the project directory**

```bash
cd "Hotel Managment System"
```

**3. Open the project**

Open the project folder in your preferred Java IDE.

**4. Run the application**

Execute the `Start.java` file to launch the application.

The login interface will appear first, followed by the management dashboard after successful authentication.

### Default Login Credentials

The current source code contains the following hardcoded administrator credentials:

| Field | Value |
|---|---|
| Username | Admin |
| Password | admin |

**Note:** These are demonstration credentials from the current implementation, not a secure production authentication system.

## 🎯 Project Objectives

The primary objectives of this project are:

- To develop a functional desktop-based hotel administration application using Java.
- To implement CRUD operations for managing hotel-related information.
- To apply Object-Oriented Programming concepts in a practical software development project.
- To develop an interactive GUI using Java Swing.
- To understand file handling and persistent data management in Java.
- To organize application components using modular programming principles.

## 🔮 Future Improvements

Potential enhancements for future versions include:

- Integration with a relational database such as MySQL.
- Secure authentication with password hashing.
- Complete room reservation and booking management.
- Check-in and check-out management.
- Payment processing and invoice generation.
- Advanced reporting and analytics.
- Improved input validation and error handling.
- Dynamic data structures for handling larger datasets.

## 👨‍💻 Author

**Sazzadul Haque Chowdhury**

GitHub: [Sazzadul-Haque-Chowdhury](https://github.com/Sazzadul-Haque-Chowdhury)

**Project:** Hotel Management System

**Language:** Java

---

⭐ If you find this project interesting, feel free to explore the repository!
