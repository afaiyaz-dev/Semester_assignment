# 🏦 Bank Management System (C++ OOP)

A console-based Bank Management System developed in C++ using Object-Oriented Programming (OOP) principles. Designed to simulate real-world banking operations across Customer, Admin, and ATM interfaces with persistent file storage.

## ✨ Key Features

### 👤 Customer Portal
- **Account Creation:** Open a **Savings** or **Current** account with auto-generated account numbers and 4-digit PIN security.
- **Core Transactions:** Deposit, withdraw, and transfer funds between accounts with balance and overdraft validation.
- **Mini Statement:** View timestamped transaction history for deposits, withdrawals, and transfers.
- **Account Management:** View profile details and update security PINs.

### 🛡️ Bank Admin Portal
- **Account Directory:** View all registered accounts in a formatted table and search by Account Number or Holder Name.
- **Security Controls:** Freeze or unfreeze accounts to restrict unauthorized access.
- **Account Lifecycle:** Close zero-balance accounts and apply batch interest across all Savings accounts.

### 🏧 ATM Simulation Mode
- **Fast Cash & Custom Withdrawals:** Quick preset withdrawal options alongside standard cash withdrawal.
- **Security Protections:** Daily withdrawal limits and automatic account lockout after 3 consecutive failed PIN attempts.

## 🧠 OOP Concepts & Technical Highlights
- **Abstraction & Polymorphism:** Abstract `Account` base class with virtual methods (`withdraw()`, `calculateInterest()`) overridden by derived classes.
- **Inheritance:** Specialized `SavingsAccount` (interest calculation, minimum balance rules) and `CurrentAccount` (overdraft support).
- **Encapsulation:** Protected account credentials, PIN masking, and controlled balance mutations.
- **Composition:** `Bank` controller managing `Account` objects, each maintaining a history of `Transaction` records.
- **File Persistence:** Automatic data serialization and loading using `<fstream>` so records persist across sessions.

## 🛠️ Tech Stack
- **Language:** C++ (STL `vector`, `fstream`, `ctime`)
- **Paradigm:** Object-Oriented Programming (OOP)

## 🚀 Getting Started

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
   cd your-repo-name
