# 💳 Banking System using Python, Tkinter & SQLite

A modern **Banking Management System** built in **Python** with an interactive **Tkinter GUI** and **SQLite database**.  
The system integrates the **Merge Sort algorithm** (O(n log n)) from the **Design and Analysis of Algorithm (DAA)** domain to efficiently sort financial records like transactions and user accounts.

---

## 📘 Project Overview

The **Banking System** is designed to simulate core banking operations such as account creation, login, deposits, withdrawals, fund transfers, and transaction tracking.  
It provides separate dashboards for **Users** and **Admins**, enabling both individual account management and system-wide monitoring.  

From an algorithmic perspective, this project demonstrates how the **Merge Sort** algorithm enhances data handling efficiency within financial applications.

---

## 🧠 Design and Analysis of Algorithm Component

### 🔹 Algorithm Used: Merge Sort

The **Merge Sort algorithm** is implemented to:
- Sort user transactions by timestamp (latest first)  
- Sort account lists alphabetically by username  
- Sort admin statements globally for better readability  

This ensures **stable and efficient sorting** with consistent **O(n log n)** performance, even for large datasets.

---

## 🧩 System Architecture

```
+------------------------------------------------------------+
|                      BANKING SYSTEM                        |
+------------------------------------------------------------+
|                            GUI                             |
|                    (Tkinter Interface)                     |
|  +------------------------------------------------------+  |
|  |  User Login | Transactions | Admin Panel | CSV Export |  |
|  +------------------------------------------------------+  |
|                                                            |
|                            ↓                               |
|                   Database Layer (SQLite)                  |
|   - Accounts Table (User Data)                             |
|   - Transactions Table (History)                           |
|   - Admin Table (Credentials)                              |
|                                                            |
|                            ↓                               |
|                Merge Sort Algorithm (DAA)                  |
|  Used for efficient sorting of transaction and account data|
+------------------------------------------------------------+
```

---

## 🚀 Features

### 👤 User Features
- Register a new account with initial deposit  
- Login securely and manage your account  
- Deposit, withdraw, or transfer funds  
- View transaction statement (sorted via Merge Sort)  
- Get real-time balance updates  

### 🧑‍💼 Admin Features
- Login using admin credentials  
- View all user accounts and balances  
- Access complete transaction history  
- Export system transactions to a CSV file  
- Automatically sorted data for better readability  

---

## 🧠 Algorithm Analysis

| Parameter | Merge Sort |
|------------|-------------|
| **Approach** | Divide and Conquer |
| **Best Case** | O(n log n) |
| **Average Case** | O(n log n) |
| **Worst Case** | O(n log n) |
| **Space Complexity** | O(n) |
| **Stability** | Stable ✅ |

---

## 🧩 Technologies Used

| Layer | Technology |
|-------|-------------|
| **Frontend (GUI)** | Python Tkinter |
| **Backend (Database)** | SQLite3 |
| **Algorithm (DAA)** | Merge Sort |
| **File Handling** | CSV Export |
| **Language** | Python 3.10+ |

---

## 🗂️ Folder Structure

```
Banking_System/
│
├── main.py
├── gui.py                      # GUI interface (User + Admin)
├── Database.py                 # Database manager (SQLite operations)
├── banking_data.db             # Auto-created database file
├── system_transactions.csv     # Exported transaction data
├── README.md                   # Project documentation
└── requirements.txt            # (Optional) Dependencies file
```

---

## ⚙️ Installation and Execution

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/akashnegi7/Banking-System.git
cd Banking-System
```

### 2️⃣ Run the Application
Ensure **Python 3.10+** is installed.
```bash
python main.py
```

### 3️⃣ Default Admin Credentials
```
Username: admin
Password: adminpass
```

---

## 🧾 Database Schema

### 🧩 Accounts Table
| Column | Type | Description |
|---------|------|-------------|
| id | INTEGER | Primary Key |
| username | TEXT | Unique user name |
| password | TEXT | User password |
| balance | REAL | Current account balance |

### 💸 Transactions Table
| Column | Type | Description |
|---------|------|-------------|
| id | INTEGER | Primary Key |
| account_id | INTEGER | Foreign key to accounts |
| type | TEXT | Deposit / Withdraw / Transfer |
| amount | REAL | Transaction amount |
| timestamp | TEXT | Date and time |
| description | TEXT | Additional transaction details |

---

## 🧪 Results

✅ User and admin interfaces operate seamlessly  
✅ Transaction and account data sorted using Merge Sort  
✅ Database persists all operations reliably via SQLite  
✅ CSV export functionality verified  
✅ Algorithm efficiency validated for large datasets (1000+ transactions)  

---

## 🌟 Future Enhancements

- Add **Quick Sort** and **Heap Sort** for performance comparison  
- Include **graphical transaction visualization (Matplotlib)**  
- Implement **password encryption** for security  
- Extend system into a **web-based version** using Flask or Django  

---

## 📚 References

1. Cormen, T. H. et al. *Introduction to Algorithms (4th ed.)*, MIT Press.  
2. Python Software Foundation — *Tkinter & SQLite3 Documentation*.  
3. John von Neumann (1945) — *Original Merge Sort Algorithm*.  
4. Sedgewick, R. & Wayne, K. *Algorithms (4th ed.)*, Addison-Wesley.  

---

## 👨‍💻 Author

**Akash Singh Negi**  
🎓 Data Science & Algorithms Enthusiast  
📫 [LinkedIn](https://www.linkedin.com/in/akash-singh-negi/) • 💻 [GitHub](https://github.com/akashnegi7)
