# 🏦 Bank Management System & ATM Simulator (Java)

A desktop banking and ATM simulation application built using **Java (Swing/AWT)** and **JDBC/MySQL**. The system replicates real-world retail banking workflows, from multi-step account creation to secure ATM transactions.

## 📌 Overview
Developed in NetBeans (`bank.management.system`), this application provides an interactive graphical interface (`atm.jpg` / `logo.jpg`) backed by a relational database (`Conn.java`)[cite: 2]. Users can register for a new bank account, receive a card number and PIN, and perform standard ATM operations with persistent transaction history[cite: 2].

## ✨ Key Features
- **3-Step Account Onboarding (`SignUp`, `SignUpTwo`, `SignUpThree`):** Collects personal details, additional KYC/demographic information, and account preferences (Savings/Current, card services)[cite: 2].
- **Secure ATM Login (`Login`):** Authenticates users via Card Number and 4-digit PIN[cite: 2].
- **Core ATM Transactions (`Transaction`):**
  - **Cash Deposit (`Deposite`):** Credit funds directly to the user's account[cite: 2].
  - **Cash Withdrawal (`Withdraw`) & Fast Cash (`FastCash`):** Withdraw custom amounts or select quick preset denominations with balance validation[cite: 2].
  - **Balance Enquiry (`BalanceEnquiry`):** Real-time calculation and display of available account balance[cite: 2].
  - **Mini Statement (`MiniStatement`):** Displays recent transaction logs[cite: 2].
  - **PIN Change (`PinChange`):** Allows users to securely update their ATM PIN[cite: 2].

## 🛠️ Tech Stack
- **Language:** Java (JDK)[cite: 2]
- **GUI Framework:** Java Swing & AWT
- **Database & Connectivity:** MySQL, JDBC (`Conn.java`)[cite: 2]
- **IDE / Build Tool:** Apache NetBeans / Ant (`build.xml`)[cite: 2]

## 📂 Project Structure
```text
src/
├── bank/management/system/
│   ├── Conn.java            # JDBC database connection handler
│   ├── Login.java           # Card & PIN authentication screen
│   ├── SignUp.java          # Step 1: Personal details form
│   ├── SignUpTwo.java       # Step 2: Additional KYC details form
│   ├── SignUpThree.java     # Step 3: Account & card setup
│   ├── Transaction.java     # Main ATM dashboard menu
│   ├── Deposite.java        # Cash deposit module
│   ├── Withdraw.java        # Cash withdrawal module
│   ├── FastCash.java        # Preset quick-withdrawal module
│   ├── BalanceEnquiry.java  # Live balance check
│   ├── MiniStatement.java   # Recent transaction history viewer
│   └── PinChange.java       # ATM PIN reset module
└── icons/
    ├── atm.jpg              # ATM interface background graphic
    └── logo.jpg             # Bank brand logo
```[cite: 2]

## 🚀 Getting Started

### Prerequisites
- **Java Development Kit (JDK 8 or higher)**
- **MySQL Server** & **MySQL Connector/J** (`.jar` added to project libraries)
- **Apache NetBeans IDE** (recommended, as `nbproject/` configuration is included)[cite: 2]

### Setup & Run
1. **Clone the repository:**
   ```bash
   git clone [https://github.com/](https://github.com/)<your-username>/bank-management-system-java.git
