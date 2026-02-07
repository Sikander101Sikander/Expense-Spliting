# Splitwise Expense Management System (C++)

A **console-based Splitwise-like application** implemented in **C++** using **Object-Oriented Programming** and **design patterns**.  
The system manages **group and individual expenses**, supports multiple **split strategies**, tracks balances, sends notifications, and simplifies debts.

---

## ✨ Features

- Create and manage users
- Create groups and add/remove members
- Add group expenses with:
  - Equal split
  - Exact split
  - Percentage split
- Add individual (one-to-one) expenses
- Automatic balance tracking
- Settle payments within groups
- Debt simplification using greedy algorithm
- Notifications using Observer pattern
- Prevent users from leaving a group with pending balances

---

## 🧠 Design Patterns Used

- **Singleton Pattern**
  - `Splitwise` class ensures a single global instance
- **Strategy Pattern**
  - `EqualSplit`, `ExactSplit`, `PercentageSplit`
- **Factory Pattern**
  - `SplitFactory` creates split strategies
- **Observer Pattern**
  - `User` receives notifications for expenses and settlements
- **Facade Pattern**
  - `Splitwise` provides a unified interface for system operations

---

## 🏗️ Core Classes

- `User` – Maintains personal balances and receives notifications
- `Group` – Manages members, expenses, and group balances
- `Expense` – Stores expense details and split data
- `Split` – Represents individual share of an expense
- `DebtSimplifier` – Optimizes debts to minimize transactions
- `Splitwise` – Main controller (Singleton + Facade)

---

## 📋 Functional Requirements

- Users can join and leave groups
- Users must clear dues before leaving a group
- Group expenses support multiple split types
- Individual expenses are supported
- Notifications are sent on expense addition and settlement
- Group debts can be simplified

---

## 🛠️ Technologies & Concepts

- **Language:** C++
- **STL Used:** `vector`, `map`, `algorithm`, `iomanip`
- **Concepts:**
  - OOP (Encapsulation, Inheritance, Polymorphism)
  - Design Patterns
  - Greedy Algorithm
  - Memory Management
  - Console-based System Design

---

## ▶️ How to Compile & Run

```bash
g++ splitwise.cpp -o splitwise
./splitwise
