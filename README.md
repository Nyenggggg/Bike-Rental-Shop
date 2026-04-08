# 🚴 Bike Rental Shop

A command-line bike rental system built using PostgreSQL and Bash scripting.
This project simulates a real-world rental service where users can rent and return bikes while tracking availability in a database.

---

## 📌 Features

* View available bikes
* Rent a bike
* Return a bike
* Track customer rentals
* Store rental history in a database

---

## 🗄️ Database Structure

The system uses a relational database with the following tables:

* `bikes` – stores bike details and availability
* `customers` – stores customer information
* `rentals` – tracks bike rentals and returns

### 🔗 Relationships

* One customer can have multiple rentals
* One bike can be rented multiple times

---

## 📦 Sample Data

The database includes preloaded bikes such as:

* Mountain Bikes
* Road Bikes
* BMX Bikes

This allows immediate testing after setup.

---

## ⚙️ How to Run

### 1. Create the database

```bash
createdb bikes
```

### 2. Import the SQL file

```bash
psql -U postgres -d bikes -f bike-shop.sql
```

### 3. Run the application

```bash
bash bike-shop.sh
```

---

## 🔍 Example Query

```sql
SELECT * FROM bikes;
```

Example output:

```
 bike_id | model          | available
---------+----------------+----------
 1       | Mountain Bike  | true
 2       | Road Bike      | false
 3       | BMX Bike       | true
```

---

## 📚 What I Learned

* SQL database design
* Table relationships and foreign keys
* CRUD operations
* Bash scripting integration with PostgreSQL

---

## 🎯 Purpose

This project was built to practice database management and simulate a real-world rental system.

---

## 👤 Author

Rienniel Lopez
