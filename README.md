# ATM_Machine_System
# ATM Management System

The ATM Management System is a console-based application designed to simulate the operations of an Automated Teller Machine (ATM).
<br>
This project is implemented using Python for the application logic and MySQL for data storage.


## Features

- **New Account Creation**: Allows users to create a new account by providing a name and PIN.
- **Account Inquiry**: Enables users to check their account details including balance.
- **Deposit**: Supports depositing money into an account.
- **Withdraw**: Allows withdrawing money from an account, given sufficient funds.
- **Account Search**: Provides the ability to search for an account by name.
- **Display All Accounts**: Lists all the accounts stored in the system.

## Getting Started

### Prerequisites

- Python 3.x
- MySQL Server
- `mysql-connector-python` package

### Installation

1. **Clone the repository**

    ```bash
    cd ATM-Management-System
    ```

2. **Set up the MySQL Database**

    - Log in to your MySQL server and create a new database named `atm_system`.
    - Execute the SQL script provided in `setup.sql` to create the necessary tables.

3. **Configure Database Connection**

    - Navigate to `db/database.py` and update the connection details:

    ```bash
    connection = mysql.connector.connect(
        host="localhost",
        user="your_username",
        password="your_password",
        database="atm_system"
    )
    ```

4. **Install Dependencies**

    ```bash
    pip install requirements.txt
    ```

### Running the Application

Run the `main.py` script from the root directory of the project:

    ```bash
    python main.py
    ```

Follow the on-screen prompts to interact with the system.

## Project Structure

```
ATMManagementSystem/
│
├── db/
│   └── database.py          # Database connection and operations
│
├── models/
│   └── account.py           # Account model class
│
├── services/
│   └── account_service.py   # Business logic for account operations
│
└── main.py                  # Main application entry point (CLI interface)
```

