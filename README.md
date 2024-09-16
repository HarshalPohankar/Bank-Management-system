Bank Management System
======================

Overview
--------
The Bank Management System is a Java application designed for managing banking operations. It features account management, transaction handling, and user authentication. The system uses Java Swing (JFrame) for the graphical user interface and MySQL for data storage.

Features
--------
- Account Management: Create, update, and delete customer accounts.
- Transaction Handling: Deposit and withdraw funds.
- User Authentication: Secure login and logout.
- Data Persistence: MySQL database integration.

Requirements
------------
- Java Development Kit (JDK) 8 or higher.
- MySQL 5.7 or higher.
- JDBC Driver for MySQL (included in the `lib` directory).
- MySQL Workbench (optional for database management).

Setup and Installation
----------------------
1. Clone the Repository:
   $ git clone https://github.com/yourusername/bank-management-system.git
   $ cd bank-management-system

2. Configure MySQL Database:
   a. Create the Database:
      CREATE DATABASE bank_db;

  

   b. Configure Database Connection:
      Edit `src/db/DatabaseConfig.java` and update the following variables with your MySQL credentials:
      - DB_URL = "jdbc:mysql://localhost:3306/bank_db"
      - DB_USER = "root"
      - DB_PASSWORD = "yourpassword"

3. Build the Project:
   Build the project using your preferred IDE (IntelliJ IDEA, Eclipse) or using command-line tools. Make sure all required libraries are included in the classpath.

4. Run the Application:
   Run the `Main` class from your IDE or using the command line:
   $ java -cp "path/to/your/libs/*:path/to/your/classes" Main

Usage
------
1. Launch the Application:
   The application will open a JFrame-based user interface.

2. Login:
   Enter your credentials to access the system.

3. Manage Accounts:
   - Create Account: Use the form to add new customers.
   - Update Account: Modify customer details.
   - Delete Account: Remove accounts as needed.

4. Perform Transactions:
   - Deposit: Add funds to an account.
   - Withdraw: Withdraw funds from an account.

5. View Transactions:
   Review the transaction history for each account.

Troubleshooting
---------------
- Database Connection Issues: Ensure MySQL is running and the credentials in `DatabaseConfig.java` are correct.
- ClassNotFoundException: Ensure the MySQL JDBC driver JAR is in the classpath.

License
-------
This project is licensed under the MIT License. See the LICENSE file for details.

