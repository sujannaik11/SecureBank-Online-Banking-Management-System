# SecureBank – Online Banking Management System

A web-based banking application developed using Python, Flask, MySQL, HTML, CSS, and JavaScript. SecureBank provides a centralized interface for managing banking activities, including account balances, fund transfers, bill payments, loans, transaction records, and account statements.

## 📌 Project Overview

SecureBank is an academic full-stack web development project designed to demonstrate the implementation of common banking workflows through a user-friendly web interface.

The application includes separate user and administrative interfaces, transaction PIN functionality, bill-payment management, recurring payment configuration, transaction analytics, and PDF statement generation.

**Note:** This is an educational project and is not a production banking platform. Transactions are simulated within the application's configured database.

## ✨ Features

### 👤 User Account Management
- User registration and login
- User profile viewing and editing
- Account dashboard
- Account balance viewing
- Transaction PIN setup and change

### 💸 Banking Operations
- Fund transfers
- Add-funds functionality
- Credit-related functionality
- Transaction history
- Balance and transaction summaries

### 🧾 Bill Payment Management
- Bill-payment interface
- Biller selection and management
- Saved billers
- Bill-payment history
- Recurring payment configuration
- Enable, disable, and delete recurring payment settings

### 📄 Account Statements
- View account statements for a selected period
- Transaction summaries
- Download PDF statements
- Print-friendly statements
- Email statement functionality, subject to email configuration

### 💰 Loan Management
- Loan application functionality
- Loan records
- Administrative loan management, where implemented

### 📊 Analytics and Administration
- Banking activity analytics
- Administrative dashboard
- User details management
- Administrative user operations

### 🔗 Additional Demonstration
- Blockchain demonstration page

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| Python | Application logic |
| Flask | Backend web framework |
| MySQL | Relational database |
| mysql-connector-python | Python–MySQL connectivity |
| HTML5 | Page structure |
| CSS3 | Styling and responsive interface |
| JavaScript | Client-side interactions |
| Jinja2 | Dynamic HTML templates through Flask |
| ReportLab | PDF statement generation |
| Flask-Mail | Email functionality |
| Werkzeug | Web utility and security functions |

## 📁 Project Structure

```text
SecureBank-Online-Banking-System/
├── app.py
├── requirements.txt
├── ACCOUNT_STATEMENTS_SETUP.md
├── BILL_PAYMENTS_SETUP.md
├── database_schema_bills.sql
├── init_bill_tables.py
├── templates/
│   ├── base.html
│   ├── dashboard.html
│   ├── signup.html
│   ├── login.html
│   ├── profile.html
│   ├── balance.html
│   ├── transfer.html
│   ├── history.html
│   ├── loan.html
│   ├── bills.html
│   ├── pay_bill.html
│   ├── recurring_payments.html
│   ├── statements.html
│   ├── analytics.html
│   └── admin.html
└── static/
    ├── css/
    │   └── style.css
    ├── js/
    │   └── script.js
    └── images/
```

*The structure above highlights the main files; the repository also contains additional templates and supporting files.*

## ⚙️ Installation and Setup

### Prerequisites

Install the following before running the project:

- Python 3.10 or a compatible Python version
- MySQL Server
- MySQL Workbench (optional, for database management)
- Git (optional)

### Step 1: Download the project

Download the repository as a ZIP file from GitHub and extract it, or clone it using:

```bash
git clone https://github.com/YOUR_USERNAME/SecureBank-Online-Banking-System.git
cd SecureBank-Online-Banking-System
```

### Step 2: Create a virtual environment

```bash
python -m venv venv
```

Activate it on Windows:

```powershell
.\venv\Scripts\Activate.ps1
```

If PowerShell blocks activation, you can use:

```powershell
.\venv\Scripts\python.exe -m pip install -r requirements.txt
```

### Step 3: Install dependencies

```bash
python -m pip install -r requirements.txt
```

### Step 4: Configure MySQL

1. Start your MySQL server.
2. Create the database required by the application.
3. Configure the database connection settings in `app.py`, or preferably use environment variables.
4. Run any required SQL setup scripts, including `database_schema_bills.sql`, using MySQL Workbench or the MySQL command line.

The application is configured to use a MySQL database named `online_banking`. Verify the database name, username, password, host, and required tables before starting the application.

**Important:** Do not publish your real database password or other credentials. Use local environment variables or a private configuration file excluded from Git.

### Step 5: Configure email functionality (optional)

If you want to use email-based statement delivery, configure the required Flask-Mail SMTP settings and credentials. Email functionality will not work until the mail settings are valid.

### Step 6: Run the application

From the project directory, execute:

```bash
python app.py
```

Open the local address displayed in the terminal, commonly:

```text
http://127.0.0.1:5000
```

Use the registration page to create a test account, or configure the appropriate administrative account according to your application's setup.

## 🔐 Security Considerations

- Never commit passwords, API keys, SMTP credentials, or secret keys.
- Use environment variables for sensitive configuration.
- Use strong password hashing and secure session configuration.
- Validate user input and enforce authorization for every banking operation.
- Test transaction handling, balance updates, and concurrent requests carefully.
- Use only dummy data; do not store real customer or banking information.
- Do not deploy this academic prototype for real financial transactions.

## 🧪 Testing

Test the following workflows before presenting or demonstrating the application:

- User registration, login, and logout
- Account balance display
- Fund transfers and transaction history
- Transaction PIN validation
- Bill payments and saved billers
- Recurring payment settings
- Statement generation and PDF download
- Email delivery after SMTP configuration
- Administrative access restrictions

## 🎓 Project Purpose

This project demonstrates practical concepts in full-stack web development, relational database integration, session-based authentication, transaction processing, report generation, and administrative dashboard development.

It can be extended with automated tests, stronger security controls, improved transaction consistency, and integration with authorized payment APIs.

## 👨‍💻 Author

**Sujan**

Computer Science and Engineering

## 📄 License

No license has been specified for this project. All rights remain with the respective copyright holder unless a license is added.
