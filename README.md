# EmployeeManagementSystem

Employee Management System (Core Java)
Overview

The Employee Management System is a console-based Java application designed to manage employee records efficiently.
It demonstrates the use of Core Java, Object-Oriented Programming (OOP) concepts, Collections Framework, and File I/O for data persistence.

Purpose

To perform basic CRUD (Create, Read, Update, Delete) operations on employee records using HashMap and Serialization in Java.

⚙️ Features

✅ Add new employee records
✅ View all employee records
✅ Update existing employee details
✅ Delete employee records
✅ Save and load data using file handling (serialization)
✅ Menu-driven console interface

Concepts Covered

Core Java

OOP Principles (Encapsulation, Abstraction)

Collections Framework (HashMap)

File I/O (Object Serialization)

Exception Handling

Switch-Case + Scanner (User Input)

 Project Structure
EmployeeManagementSystem/
│
├── src/
│   └── com/ems/
│       ├── Employee.java
│       ├── EmployeeService.java
│       └── EmployeeManagementApp.java
│
├── employees.dat          # Auto-generated file for saving employee data
│
└── README.md

Class Details
Employee.java

Represents an Employee entity with fields:

id (int)

name (String)

department (String)

salary (double)

Implements Serializable to allow saving employee data to a file.

EmployeeService.java

Contains business logic using a HashMap<Integer, Employee> for CRUD operations:

addEmployee()

viewAllEmployees()

updateEmployee()

deleteEmployee()

Also includes:

saveToFile() → Serializes employee data to employees.dat

loadFromFile() → Loads existing employee data when the program starts

EmployeeManagementApp.java

Acts as the main class containing a menu-driven program that interacts with the user via the console using Scanner and switch-case statements.

 How to Run
🛠️ Prerequisites

Java JDK 8 or higher

Eclipse IDE or IntelliJ IDEA

Steps

Open Eclipse or IntelliJ IDEA.

Create a new Java Project named EmployeeManagementSystem.

Create a package named com.ems.

Add the three Java files (Employee.java, EmployeeService.java, EmployeeManagementApp.java) to the package.

Run the EmployeeManagementApp class.

Sample Console Output
===== Employee Management System =====
1. Add Employee
2. View All Employees
3. Update Employee
4. Delete Employee
5. Exit
Enter your choice: 1
Enter ID: 101
Enter Name: Umang
Enter Department: IT
Enter Salary: 55000
Employee added successfully!

Data Storage

All employee data is saved to a serialized file named employees.dat.
This ensures that data persists between program runs.

Learning Outcomes

By building this project, you’ll learn how to:

Design classes using OOP principles

Use HashMap for storing and managing data

Implement CRUD operations

Perform file read/write operations

Handle user input in console-based Java apps
