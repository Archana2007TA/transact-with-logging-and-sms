# 🧾 Bank Account Management System with SMS & Logging

This project is a Python-based **Bank Account Management System** with integrated **logging** and **SMS notifications** (via Twilio). It allows users to perform basic banking operations like **withdrawals** and **deposits**, while logging each transaction, error, and alert to a file for full traceability.

## ✅ Key Features

- 🔐 Custom exception handling for invalid transactions
- 🧾 Full **logging integration** (INFO, WARNING, ERROR, CRITICAL)
- 💬 Real-time **SMS alerts** using Twilio API
- 📥 Clean, readable code for educational or prototype use

---

## 📝 Logging System Overview

This project uses Python's built-in `logging` module to track every key activity. All logs are written to `bank_transactions.log` for record-keeping, debugging, and auditing purposes.

### 🔍 Log Configuration

```python
logging.basicConfig(filename='bank_transactions.log', level=logging.INFO)

| Level      | Purpose                                                      |
| ---------- | ------------------------------------------------------------ |
| `INFO`     | Logs successful transactions and operations                  |
| `WARNING`  | Logs failed operations (e.g., invalid deposit or withdrawal) |
| `ERROR`    | Logs issues like SMS failures or unexpected exceptions       |
| `CRITICAL` | Logs severe or unexpected program-level errors               |
