# 🏥 AI-Powered OPD Insurance Claims Adjudication System

An intelligent insurance claim adjudication platform that automates outpatient (OPD) claim processing using AI-powered document extraction, rule-based policy validation, fraud detection, and automated decision-making.

## 🚀 Overview

Insurance claim processing is often manual, time-consuming, and prone to inconsistencies. This project streamlines the adjudication workflow by combining:

* AI-based medical document extraction
* Policy rule validation
* Fraud detection mechanisms
* Automated approval/rejection decisions
* Confidence scoring
* Claim history tracking

The system can process prescriptions, medical bills, and diagnostic reports, automatically extracting relevant information and evaluating claims against policy rules.

---

## ✨ Features

### 📄 AI Document Extraction

* Upload medical bills, prescriptions, and reports
* OCR-based text extraction using Tesseract.js
* Structured data extraction using Groq LLM
* Automatic form population

### ⚙️ Rule-Based Adjudication Engine

* Eligibility verification
* Waiting period validation
* Policy coverage checks
* Sub-limit validation
* Per-claim limit enforcement
* Network hospital benefits
* Copay calculation

### 🚨 Fraud Detection

* Multiple claims on the same day
* Unusual claim patterns
* High-value claim flagging
* Manual review escalation

### 🏥 Healthcare Policy Support

* Network hospital discounts
* Cashless claim processing
* Consultation limits
* Pharmacy limits
* Diagnostic limits
* Dental coverage
* Alternative medicine coverage

### 📊 Analytics Dashboard

* Claim history
* Approval statistics
* Rejection trends
* Confidence scores
* Decision explanations

---

## 🧠 Adjudication Workflow

### Step 1: Eligibility Validation

* Policy active check
* Minimum claim amount validation
* Submission deadline verification
* Waiting period validation

### Step 2: Document Verification

* Prescription verification
* Doctor registration validation
* Medical bill verification

### Step 3: Coverage Validation

* Exclusion checks
* Service coverage verification
* Pre-authorization requirements

### Step 4: Financial Validation

* Per-claim limits
* Sub-limit calculations
* Copay deductions
* Network discounts

### Step 5: Medical Necessity Review

* Diagnosis validation
* Procedure justification
* Treatment relevance checks

### Step 6: Fraud Detection

* Duplicate claim detection
* Suspicious activity checks
* Risk flag generation

---

## 📋 Supported Decisions

### ✅ APPROVED

Claim satisfies all policy requirements.

### ◑ PARTIAL APPROVAL

Some claim components are covered while others are excluded.

### ❌ REJECTED

Claim violates policy rules or lacks required documentation.

### 🔍 MANUAL REVIEW

Claim requires human review due to fraud indicators or exceptional circumstances.

---

## 🏗️ Architecture

```text
Medical Documents
       │
       ▼
Tesseract OCR
       │
       ▼
Groq LLM Extraction
       │
       ▼
Structured Claim Data
       │
       ▼
Adjudication Engine
       │
       ▼
Policy Validation
       │
       ▼
Fraud Detection
       │
       ▼
Decision Engine
       │
       ▼
Final Claim Outcome
```

---

## 🛠️ Tech Stack

### Frontend

* React.js
* Vite
* JavaScript

### AI & OCR

* Tesseract.js
* Groq API
* Llama 3.3 70B

### Business Logic

* Custom Rule Engine
* Policy Validation Engine
* Fraud Detection Module

### Deployment

* Vercel

---

## 📂 Project Structure

```text
plum-opd-adjudication/

├── App.jsx
├── main.jsx
├── index.css
├── index.html
├── package.json
├── vite.config.js
├── README.md
└── opd screenshot/
```

---

## ⚙️ Installation

### Clone Repository

```bash
git clone <repository-url>
cd plum-opd-adjudication
```

### Install Dependencies

```bash
npm install
```

### Install OCR Library

```bash
npm install tesseract.js
```

### Run Development Server

```bash
npm run dev
```

---

## 🔑 API Configuration

Obtain a Groq API key:

1. Create an account on Groq Console
2. Generate an API key
3. Launch the application
4. Click **Add API Key**
5. Paste your Groq API key

The key remains in the browser and is never stored on any server.

---

## 🧪 Test Cases

The application includes 10 predefined test scenarios:

| Test Case                 | Expected Result  |
| ------------------------- | ---------------- |
| Simple Consultation       | Approved         |
| Dental Treatment          | Partial Approval |
| Limit Exceeded            | Rejected         |
| Missing Documents         | Rejected         |
| Waiting Period Violation  | Rejected         |
| Alternative Medicine      | Approved         |
| Missing Pre-Authorization | Rejected         |
| Fraud Detection           | Manual Review    |
| Excluded Treatment        | Rejected         |
| Network Cashless Claim    | Approved         |

---

## 📈 Key Business Rules

### Financial Limits

| Coverage Type        | Limit   |
| -------------------- | ------- |
| Annual Limit         | ₹50,000 |
| Per Claim Limit      | ₹5,000  |
| Consultation         | ₹2,000  |
| Pharmacy             | ₹15,000 |
| Diagnostics          | ₹10,000 |
| Dental               | ₹10,000 |
| Vision               | ₹5,000  |
| Alternative Medicine | ₹8,000  |

### Policy Conditions

* 10% Copay
* 20% Network Hospital Discount
* 30-Day Submission Window
* Waiting Period Validation
* Fraud Monitoring

---

## 🎯 Future Enhancements

* FastAPI Backend
* PostgreSQL Database
* User Authentication
* Audit Logging
* PDF Report Generation
* Advanced Fraud Scoring
* Multi-Policy Support
* Real-Time Notifications
* Admin Dashboard
* Explainable AI Decisions

---

## 📸 Screenshots

Add screenshots from the application inside the `opd screenshot` folder and reference them here.

---

## 👨‍💻 Author

Navadeep Kandru

B.Tech – Computer Science & Engineering

Interests:

* Machine Learning
* Deep Learning
* Generative AI
* Data Science
* Intelligent Decision Systems

---

## 📜 License

This project is intended for educational, research, and demonstration purposes.
