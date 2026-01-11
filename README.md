Here’s a clean, professional **README.md** for your project 👇
(You can copy-paste this directly into a `README.md` file)

---

# 🏨 Hotel Reservation System (Java + MySQL)

A **console-based Hotel Reservation System** built using **Java and JDBC** that allows hotel staff to manage room reservations efficiently using a MySQL database.

This application supports:

* Creating reservations
* Viewing all reservations
* Fetching room numbers
* Updating reservations
* Deleting reservations

---

## 🚀 Features

* 📌 Reserve a hotel room
* 📋 View all current reservations
* 🔍 Find room number by Reservation ID & Guest Name
* ✏️ Update reservation details
* 🗑️ Delete a reservation
* 💾 Data stored permanently in MySQL
* 🔒 Validates reservation existence before update/delete

---

## 🛠️ Technologies Used

| Technology         | Purpose                  |
| ------------------ | ------------------------ |
| Java               | Application logic        |
| JDBC               | Database connectivity    |
| MySQL              | Database                 |
| MySQL Connector/J  | JDBC Driver              |
| IntelliJ / Eclipse | IDE (any Java IDE works) |

---

## 🗄️ Database Setup

### 1️⃣ Create Database

```sql
CREATE DATABASE hostel_db;
USE hostel_db;
```

### 2️⃣ Create Table

```sql
CREATE TABLE reservations (
    reservation_id INT PRIMARY KEY AUTO_INCREMENT,
    guest_name VARCHAR(100) NOT NULL,
    room_number INT NOT NULL,
    contact_number VARCHAR(10) NOT NULL,
    reservation_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
```

---

## 🔧 JDBC Configuration

Update these values inside `HotelReservationSystem.java`:

```java
private static String url = "jdbc:mysql://localhost:3306/hostel_db";
private static String user = "root";
private static String password = "your_mysql_password";
```

---

## 📦 Required JAR

Download **MySQL Connector/J** and add it to your project:

🔗 [https://dev.mysql.com/downloads/connector/j/](https://dev.mysql.com/downloads/connector/j/)

Add it to your IDE classpath.

---

## ▶️ How to Run

1. Start MySQL Server
2. Create the database and table
3. Open the project in IDE
4. Run:

```java
HotelReservationSystem.java
```

---

## 🧭 Menu Options

```
HOTEL MANAGEMENT SYSTEM
1. Reserve a room
2. View Reservations
3. Get Room Number
4. Update Reservations
5. Delete Reservations
0. Exit
```

---

## 🧪 Sample Flow

1. Choose **1** → Enter guest name, room number, contact
2. Choose **2** → View all bookings
3. Choose **3** → Enter reservation ID and guest name
4. Choose **4** → Modify reservation
5. Choose **5** → Delete a booking

---

## 🔐 Data Safety

* Checks if reservation exists before updating or deleting
* Prevents invalid operations

---

## 📈 Future Enhancements

* PreparedStatement (to avoid SQL Injection)
* Admin login
* Room availability tracking
* GUI / Web version
* Payment integration

---

## 👨‍💻 Author

**Venkateswararao Gandrothu**
Java Full Stack Developer

