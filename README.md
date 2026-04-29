📌 Digital Complaint Registration System

A desktop-based application developed using Java Swing, DBC, and MySQL that allows users to register and manage complaints efficiently.

🚀 Features

* 🔐 User Login System
* 📝 Register New Complaints
* 📊 View All Complaints
* 💾 Data stored in MySQL database
* 🎯 Simple and user-friendly interface

 🛠️ Technologies Used

Java (Swing) – UI Development
JDBC (Java Database Connectivity) – Database connection
MySQL – Database management
Eclipse IDE– Development environment

🗄️ Database Setup

Run the following SQL queries in MySQL:

sql
CREATE DATABASE complaint_db;

USE complaint_db;

CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    username VARCHAR(50),
    password VARCHAR(50)
);

CREATE TABLE complaints (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    email VARCHAR(100),
    complaint TEXT,
    status VARCHAR(50)
);

INSERT INTO users(username, password) VALUES ('admin', 'admin123');

⚙️ How to Run the Project

1. Clone the repository:

   bash
   git clone https://github.com/your-username/your-repo-name.git


2. Open the project in Eclipse

3. Add MySQL Connector JAR to Build Path

4. Update database credentials in:

 java
 DBConnection.java
  
5. Run:
   LoginPage.java



 🔐 Default Login Credentials

Username: admin
Password: admin123


 📁 Project Structure

DigitalComplaintRegister/
│── src/com/project/
│   ├── DBConnection.java
│   ├── LoginPage.java
│   ├── Dashboard.java
│   ├── ComplaintForm.java
│   └── ViewComplaints.java


🎯 Future Enhancements

* Admin panel to update complaint status
* Password encryption for better security
* Search and filter complaints
* Improved UI using layout managers

👨‍💻 Author

Nikath Jahan 
