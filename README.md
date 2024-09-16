# Banking Management System

## Overview
This project demonstrates the use of **Java Database Connectivity (JDBC)** for interacting with a **MySQL database** in a simple **Banking Management System**. Users can register, log in, and perform basic banking operations like opening an account, crediting/debiting money, transferring funds, and checking account balances.

## Features
- User Registration and Login
- Account Creation
- Credit Money
- Debit Money
- Transfer Money between Accounts
- Balance Inquiry

## Technologies Used
- Java
- JDBC (Java Database Connectivity)
- MySQL
- JDBC Driver (MySQL Connector/J)

## Database Schema
The database consists of two main tables:
1. `user` – Stores user information like full name, email, and password.
2. `accounts` – Stores account details such as account number, balance, and security pin.

### Example Table Schema:

```sql
CREATE TABLE user (
    id INT AUTO_INCREMENT PRIMARY KEY,
    full_name VARCHAR(100),
    email VARCHAR(100) UNIQUE,
    password VARCHAR(100)
);

CREATE TABLE accounts (
    account_number BIGINT PRIMARY KEY,
    full_name VARCHAR(100),
    email VARCHAR(100),
    balance DOUBLE,
    security_pin VARCHAR(6)
);
