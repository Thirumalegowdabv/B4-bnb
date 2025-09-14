FundFlow – Transparent Finance Tracker

FundFlow is a web-based platform that brings clarity and trust to institutional finances. It visualizes the flow of funds from budgets to departments, projects, and vendors while ensuring data authenticity through hash verification.

🌟 Features

Dashboard Overview: High-level view of total budget, department allocations, and transactions.

Departments: List of all departments and their allocated budgets.

Department Details: Projects and vendors under each department.

Projects: Overview of all projects and their vendors.

Transaction Verification: Verify the integrity of transactions using SHA-256 hashes.

Interactive Charts: Pie charts to visualize budget allocation across departments.

Search & Filter: Search transactions by department or vendor.

Responsive UI: Works on desktop, tablet, and mobile.

🛠 Tech Stack

Frontend: React, Recharts, Axios

Backend: Node.js, Express.js

Database: MongoDB

Security: SHA-256 hashing for transaction integrity

Project Structure

Backend Folder Structure
```
backend/
├─ models/
│ ├─ Budget.js
│ ├─ Department.js
│ ├─ Project.js
│ ├─ Vendor.js
│ └─ Transaction.js
├─ routes/
│ ├─ auth.js
│ ├─ budget.js
│ ├─ departments.js
│ ├─ projects.js
│ ├─ vendors.js
│ └─ transactions.js
├─ controllers/
│ ├─ budgetController.js
│ ├─ departmentController.js
│ ├─ projectController.js
│ ├─ vendorController.js
│ └─ transactionController.js
├─ utils/
│ └─ hash.js
└─ server.js
```

Frontend Folder Structure
```
frontend/
├── node_modules/
├── public/
├── src/
│   ├── api/
│   ├── Components/
│   │   ├── Button/
│   │   ├── Chart/
│   │   ├── Dashboard/
│   │   ├── Department/
│   │   ├── Expenses/
│   │   ├── Form/
│   │   ├── Income/
│   │   ├── IncomeItem/
│   │   ├── Navigation/
│   │   │   └── Navigation.jsx
│   │   ├── Orb/
│   │   ├── TransactionList.jsx
│   │   └── VerifyButton.jsx
│   ├── context/
│   ├── History/
│   ├── img/
│   ├── services/
│   ├── styles/
│   ├── utils/
│   ├── App.js
│   └── index.js
├── package.json
├── package-lock.json
├── README.md
└── .gitignore
```

🚀 Setup & Run

Backend cd backend npm install node server.js

cd frontend npm install npm install crypto-js npm start

Frontend runs at http://localhost:3000 and backend at http://localhost:5000.

📌 Usage

Upload budget, departments, projects, vendors, and transactions via backend API.

View Dashboard for budget breakdown.

Click Verify on transactions to check authenticity.

Search departments/projects/vendors instantly.

🎯 Hackathon Highlights

Clarity: Easy-to-follow charts and hierarchy

Trust: Tamper-proof transactions with verification

Accessibility: Plain-English summaries for non-technical users

Feasible MVP: Built with skills our team already has

> Note: For simplicity, .env and node_modules/ are ignored in the folder structure since they are environment-specific and auto-generated.
