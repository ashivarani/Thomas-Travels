# 🚗 Thomas Travels – Driver Management System

## 📌 Project Description

**Thomas Travels** is a simple, console-based Java mini project that demonstrates how to organize and retrieve driver information for a travel service. It uses **object-oriented programming (OOP)** and Java's **ArrayList** to store sample driver records and perform basic operations on them.

The project allows you to check whether a driver belongs to the car category, find a driver by ID, count or list drivers by category, and identify the driver who has travelled the greatest total distance.

## ✨ Features

- 🚘 **Car Driver Check:** Determine whether a driver belongs to the `Car` category.
- 🔎 **Search by Driver ID:** Retrieve a driver's name, category, and total distance using their ID.
- 🔢 **Count Drivers by Category:** Count drivers in a category such as `Car`, `Auto`, or `Lorry`.
- 📋 **Filter Drivers by Category:** Retrieve all drivers belonging to a specified category.
- 🏆 **Maximum Distance Travelled:** Find the driver with the highest recorded total distance.
- 💻 **Console Output:** Display results through a Java `main` method.

Category comparisons are **case-insensitive**, so `car` and `Car` are treated as the same category.

## 🛠️ Technologies Used

| Technology | Purpose |
| --- | --- |
| Java | Application logic |
| Object-Oriented Programming | Driver model and travel operations |
| ArrayList | Store and process driver records |
| Java Development Kit (JDK) | Compile and run the application |

The project uses standard Java libraries and does not require external dependencies.

## 📂 Project Structure

```text
Thomas-Travels-main/
├── README.md
├── src/
│   └── com/
│       ├── Driver.java
│       ├── Travel.java
│       └── TestDriver.java
└── bin/
    └── com/
        ├── Driver.class
        ├── Travel.class
        └── TestDriver.class
```

### Main Classes

- **`Driver.java`** – Defines the driver model, including driver ID, name, category, and total distance travelled. Contains constructors, getters, setters, and a `toString()` method.
- **`Travel.java`** – Implements methods to search, count, filter, and evaluate drivers.
- **`TestDriver.java`** – Contains the `main()` method, creates six sample driver records, and displays the results of the operations.

## ⚙️ Core Methods

| Method | Function |
| --- | --- |
| `isCarDriver(Driver driver)` | Checks whether the driver category is `Car` |
| `retrivebyDriverId(ArrayList<Driver> driver, int id)` | Returns driver details for a given ID or a not-found message |
| `retriveCountOfDriver(ArrayList<Driver> driver, String category)` | Counts drivers in a given category |
| `retriveDriver(ArrayList<Driver> driver, String category)` | Returns drivers belonging to a given category |
| `retriveMaximumDistanceTravelledDriver(ArrayList<Driver> driver)` | Returns the driver with the greatest total distance |

The method names above are shown exactly as they appear in the existing source code.

## 🚀 How to Run

### Prerequisites

- Java Development Kit (JDK) installed
- A terminal or Java IDE (such as Eclipse, IntelliJ IDEA, or VS Code)

### Step 1: Get the Project

Download the repository ZIP from GitHub and extract it, or clone the repository using its GitHub URL.

### Step 2: Open a Terminal

Navigate to the extracted project folder containing `src` and `README.md`.

### Step 3: Compile

```bash
javac -d out src/com/Driver.java src/com/Travel.java src/com/TestDriver.java
```

### Step 4: Run

```bash
java -cp out com.TestDriver
```

The program executes the examples defined in `TestDriver.java` and prints their results in the terminal.

## 🖥️ Sample Output

```text
Is Car : true
Driver name is Baratha Belonging to the category Auto traveled 7013.0 KM so far
Count of drivers: 2
Array list of drivers in the category:
[Driver [category=Lorry, driverId=3, totalDistance=6000.0, driverName=Sugriva], Driver [category=Lorry, driverId=4, totalDistance=99400.0, driverName=Hanuman]]
Max distance travelled Driver:
Driver [category=Lorry, driverId=4, totalDistance=99400.0, driverName=Hanuman]
```

## 🎯 Learning Outcomes

This mini project demonstrates:

- Creating Java classes with constructors, getters, and setters.
- Applying encapsulation and basic object-oriented programming concepts.
- Storing objects in an `ArrayList`.
- Iterating through collections to search, count, and filter records.
- Comparing strings without case sensitivity.
- Finding a maximum value within a collection.

## 📌 Current Project Scope

The application works with **six sample drivers defined directly in `TestDriver.java`**. It runs in the console and does not currently include an interactive menu, database storage, customer bookings, or a graphical interface.

## 📝 Conclusion

**Thomas Travels** is a beginner-friendly Java mini project demonstrating basic driver record management using OOP and collections. It provides practical examples of searching, filtering, counting, and comparing driver information in a simple console application.
