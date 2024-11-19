# ATM Management System

This project is a console-based **ATM Management System** written in C. It provides a platform for users to manage their bank accounts, perform transactions, and handle account-related actions. The project is designed to test and demonstrate programming logic, file manipulation, and data handling in C.

---

## Features

### Implemented Features
1. **Login/Register**
   - Register new users (unique names).
   - Secure login with a username and password.

2. **Account Management**
   - Create new accounts.
   - View the list of owned accounts.

### Additional Features (To Be Implemented)
3. **Update Account Information**
   - Update the country or phone number of an existing account.

4. **Check Account Details**
   - View details of a specific account.
   - Display interest rates for applicable accounts:
     - **Savings**: 7%
     - **Fixed01 (1 year)**: 4%
     - **Fixed02 (2 years)**: 5%
     - **Fixed03 (3 years)**: 8%
     - **Current**: No interest.

5. **Make Transactions**
   - Deposit or withdraw money.
   - Restrictions:
     - Fixed accounts (Fixed01, Fixed02, Fixed03) cannot perform transactions.

6. **Remove Existing Accounts**
   - Delete a user’s account.

7. **Transfer Ownership**
   - Transfer an account to another user.
   - Save changes to the corresponding file.

---

## Bonus Features (Optional)
- **Real-time Notification for Ownership Transfers**  
  Using pipes and child processes to alert users instantly when they receive an account transfer.
  
- **Enhanced Security**  
  Encrypt user passwords for secure storage.

- **Improved User Interface**  
  Design a better terminal-based user interface (TUI) for a more interactive experience.

- **Relational Database Support**  
  Integrate with SQLite for improved data handling and querying.

---

## Project Structure

```plaintext
.
├── data
│   ├── records.txt     # Stores account information
│   └── users.txt       # Stores user credentials
├── Makefile            # Automates the build process
└── src
    ├── auth.c          # Handles authentication (login/register)
    ├── header.h        # Header file with declarations
    ├── main.c          # Entry point of the application
    └── system.c        # Core application logic
