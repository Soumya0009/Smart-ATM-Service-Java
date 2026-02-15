# 🏦 Smart ATM System (Java Console Application)

A console-based **Smart ATM System** built using Core Java.
This project simulates real-world ATM operations including authentication, balance inquiry, withdrawal, deposit, and transaction history management.

---

## 📌 Features

* 🔐 Account Number Authentication
* 🔑 PIN Verification
* 💰 Balance Inquiry
* 💸 Cash Withdrawal
* 💵 Cash Deposit
* 📜 Transaction History
* 🔁 Continuous Session Until Exit
* 🧠 In-Memory Database using `HashMap`

---

## 🏗️ Project Structure

```
Smart-ATM/
│
├── Main.java
│
└── ATM/
    ├── AccountATM.java
    ├── ServiceATM.java
    └── UserATM.java
```

---

## 🧱 Architecture Overview

### 1️⃣ AccountATM (Model Layer)

Represents a bank account.

**Responsibilities:**

* Store account holder details
* Manage balance
* Validate withdraw & deposit
* Maintain transaction history

---

### 2️⃣ ServiceATM (Service Layer)

Handles business logic and user interaction.

**Responsibilities:**

* Initialize users (Mock database)
* Authenticate account
* Verify PIN
* Process transactions
* Display menu options

---

### 3️⃣ UserATM (Interface)

Defines core ATM operations.

```java
public interface UserATM {
    void getInfo() throws InterruptedException;
}
```

---

## 👤 Predefined Users (Mock Database)

| Account Number | Name             | PIN  | Balance    |
| -------------- | ---------------- | ---- | ---------- |
| 123456789      | Jhon Smith       | 1234 | ₹4,000,000 |
| 234567891      | Sachin Tendulkar | 4567 | ₹5,000,000 |
| 345678901      | Michel Jaction   | 1212 | ₹6,000,000 |

---

## 🔄 ATM Workflow

1. Enter Account Number
2. Validate Account
3. Enter PIN
4. Select Service:

   * 1️⃣ Balance Check
   * 2️⃣ Withdraw
   * 3️⃣ Deposit
   * 4️⃣ Transaction History
   * 5️⃣ Exit
5. Session continues until Exit

---

## 🛠️ Technologies Used

* Java (Core Java)
* OOP Principles
* Collections Framework (`HashMap`, `ArrayList`)
* Exception Handling
* Modern Switch Expression (`case ->`)

---

## 🧠 OOP Concepts Used

* Encapsulation
* Abstraction (Interface)
* Separation of Concerns
* Method Overloading
* Constructor Initialization

---

## 🚀 How to Run

### 1️⃣ Compile

```bash
javac Main.java ATM/*.java
```

### 2️⃣ Run

```bash
java Main
```

---

## 🔒 Security Considerations

* PIN is not exposed in `toString()`
* Negative and zero transactions are blocked
* Withdrawal fails on insufficient balance
* Transactions stored per account

---

## 📈 Future Improvements

* Add transaction timestamps
* Add daily withdrawal limit
* Convert to Spring Boot REST API
* Connect with real database (MySQL/PostgreSQL)
* Add logging system
* Add card number simulation

---

## 🎯 Learning Outcomes

This project demonstrates:

* Real-world banking system logic simulation
* Service-layer design thinking
* Clean code structure
* Defensive programming
* Backend architecture fundamentals

---

## 👨‍💻 Author

**Soumya Ranjan Mohanty**
Java & Backend Developer

---
