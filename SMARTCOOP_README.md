# SMART COOP
### Web-Based Transaction and Loan Management System  
**for Paltok (SFM) Credit Cooperative**

---

## 📌 Project Overview

**SMART COOP** is a centralized, web-based transaction and loan management system developed for **Paltok (SFM) Credit Cooperative**.  
It replaces manual and decentralized online processes (Messenger, email, and personal accounts) with a **secure, role-based digital platform**.

> Blockchain integration was intentionally removed to keep the system practical, maintainable, and suitable for academic implementation.

---

## 🎯 Objectives

- Digitize cooperative transactions  
- Improve accuracy and transparency  
- Centralize member records and approvals  
- Reduce manual processing and errors  
- Provide secure role-based access  

---

## 🧑‍🤝‍🧑 User Roles

### 👤 Member
- View savings, share capital, and time deposit balances  
- Submit online deposit requests  
- Apply for loans  
- Pay loan installments  
- Upload documents for AI-powered enhancement  
- Track transaction history  

### 🧑‍💼 Employee (Staff)
- Review and approve/reject:
  - Deposits
  - Loan applications
  - Loan payments
  - Document submissions
- View members directory
- Monitor system activity

---

## 🏦 Member Accounts Logic

| Account Type | Description |
|--------------|------------|
| Savings | Maintaining balance: ₱1,000 |
| Share Capital | Non-withdrawable, visible in increments |
| Time Deposit | Withdrawable anytime |

---

## 💳 Loan Rules

- Loan ceiling = **2 × Share Capital**
- Loan terms: **3, 6, 9, 12 months**
- Co-maker required if loan exceeds share capital
- Status flow: `pending → approved / rejected`

---

## 🤖 AI Integration

- Uses **OpenCV** for document image enhancement
- Applied only to:
  - Deposit proof uploads
  - Loan payment proof uploads
- Improves readability of blurred or low-quality images

---

## 🧱 Tech Stack

**Backend**
- Python 3
- Flask
- MySQL
- OpenCV

**Frontend**
- HTML
- CSS
- JavaScript
- Jinja2

**Server**
- XAMPP (Apache & MySQL) – academic use

---

## 🗄️ Database Tables

- users  
- accounts  
- deposit_requests  
- loan_applications  
- loans  
- loan_payments  
- document_submissions  

(All tables are normalized and linked via `member_id`.)

---

## 🖥️ Dashboards

### Member Dashboard
- Home overview (advertised landing page)
- Profile & membership details
- Online deposits
- Loan application
- Loan payments
- AI document enhancement
- Transaction history

> Tabs are shown dynamically when selected.

### Employee Dashboard
- System overview
- Members directory
- Pending approvals for all transactions
- Approval/rejection with remarks

---

## 🔐 Security Features

- Session-based authentication
- Role-based access control
- Server-side validation
- Controlled file uploads
- Approval-based transaction processing

---

## 🚀 Installation (Local – Academic)

```bash
git clone https://github.com/your-username/smart-coop.git
cd smart-coop
pip install flask mysql-connector-python opencv-python
python app.py
```

Access the system at:
```
http://localhost:5000
```

---

## 📚 Academic Context

Developed as part of a **Bachelor of Science in Computer Science (BSCS)** thesis:

**SMART COOP: A Web-Based Transaction and Loan Management System with AI-Powered Document Enhancement for Paltok (SFM) Credit Cooperative**

---

## 📌 License

This project is for **academic and educational purposes only**.
