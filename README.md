# 🏥 Hospital Management System

A GUI-based Hospital Management System developed in **Python** using **Tkinter** for the user interface and **MySQL** as the backend database. This application allows users to manage patient and medicine records efficiently with full CRUD operations.

---

## 💡 Features

- ✅ Add, Update, Delete, and Search patient records
- ✅ Store medicine information (tablets, dosage, batch info)
- ✅ Integrated with MySQL for real-time database management
- ✅ Intuitive GUI built using Tkinter
- ✅ Clear and reset functionality for data entry
- ✅ Auto-population of fields on row selection
- ✅ Exception handling and validation

---

## 🛠️ Tech Stack

- **Python 3.x**
- **Tkinter** – for GUI
- **MySQL** – for database
- **mysql-connector-python** – to connect Python with MySQL

---

## 📷 Screenshots

> <img width="1357" height="716" alt="Screenshot 2025-07-26 124252" src="https://github.com/user-attachments/assets/9b7acfae-53b1-4312-9d95-0596bab72124" />


---

## 🔧 Setup & Installation

## 🚀 How to Run the App

Follow these steps to run the Hospital Management System locally on your machine.

---

### 📁 1. Clone the Repository

```bash
git clone https://github.com/yourusername/Hospital-Management-System.git
cd Hospital-Management-System
```

---

### 📦 2. Install Required Python Packages

Make sure Python 3 is installed on your system. Then install the required MySQL connector:

```bash
pip install mysql-connector-python
```

---

### 🗃️ 3. Set Up the MySQL Database

Open MySQL or XAMPP/phpMyAdmin and execute the following:

**Create the Database**

```sql
CREATE DATABASE mydata;
```

**Create the Table**

```sql
USE mydata;

CREATE TABLE hospital (
    ref VARCHAR(20) PRIMARY KEY,
    nameoftablet VARCHAR(100),
    dose VARCHAR(50),
    nooftablets VARCHAR(50),
    lot VARCHAR(50),
    issuedate VARCHAR(50),
    expdate VARCHAR(50),
    dailydose VARCHAR(50),
    storage VARCHAR(100),
    nhsnumber VARCHAR(50),
    pname VARCHAR(100),
    dob VARCHAR(50),
    address VARCHAR(200)
);
```

---

### 🔐 4. Configure MySQL Credentials

In your Python file (e.g., `Hospital management system.py`), locate the database connection and update it with your local MySQL credentials:

```python
conn = mysql.connector.connect(
    host="localhost",
    user="your_mysql_username",
    password="your_mysql_password",
    database="mydata"
)
```

---

### ▶️ 5. Run the Application

Use the terminal or command prompt to run the app:

```bash
python "Hospital management system.py"
```

A Tkinter window will open where you can interact with the system.

---
