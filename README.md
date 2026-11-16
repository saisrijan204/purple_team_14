# PURPLE — Round 2 Submission

## 1. Team Name
bugged out



## 2. Problem Statement & Solution Description

**Problem Statement:**

Users struggle to track their spending on OTT platforms, cab services, and other subscriptions. Our solution is a smart website that analyzes uploaded bank statements, automatically detects transactions from services like Netflix, Rapido, and Namma Yatri, and provides a clear breakdown of expenses to help users manage their money better.

**Proposed Solution:**

We propose developing SubSentry – an AI-powered Hidden Subscription Finder that automatically detects recurring payments from bank statements, identifies forgotten subscriptions, calculates unnecessary spending, and helps users manage or cancel subscriptions before they lose more money.



## 3. Selected Features

Your prototype must prioritize the functional implementation of **two selected features**. Other features may be represented through static UI elements and do not require functional implementation.

### Feature 1: [Feature Name]

Feature 1: Smart Transaction Detection

* Upload bank statements in PDF/CSV format.

* Automatically detect OTT, Rapido, Namma Yatri, and other subscription-related transactions.

* Categorize transactions based on service type.

### Feature 2: [Feature Name]

Feature 2: Expense Analysis & Insights

* Calculate total spending on each platform.

* Display monthly expense breakdowns using charts.

* Identify recurring subscriptions and highlight unnecessary spending.



## 4. Setup & Running Instructions

# Setup and Running Instructions

## Prerequisites
- Python 3.10 or higher
- Node.js 18 or higher
- npm
- Visual Studio Code (recommended)

## 1. Clone the Project
```bash
git clone <repository-url>
cd hidden-subscription-finder
```

## 2. Backend Setup

Navigate to the backend directory:

```bash
cd backend
```

Create a virtual environment:

```bash
python -m venv venv
```

Activate the virtual environment:

Windows:
```bash
venv\Scripts\activate
```

Install dependencies:

```bash
pip install fastapi uvicorn pymupdf pandas python-multipart pytesseract pillow
```

Install Tesseract OCR separately if scanned PDF support is required.

## 3. Run the Backend

Start the FastAPI server:

```bash
uvicorn main:app --reload
```

Backend URL:
```text
http://127.0.0.1:8000
```

API Documentation:
```text
http://127.0.0.1:8000/docs
```

## 4. Frontend Setup

Open a new terminal:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Start the frontend:

```bash
npm run dev
```

Frontend URL:
```text
http://localhost:5173
```

## 5. Application Workflow

1. Open the application in a browser.
2. Upload a bank statement in PDF format.
3. The application extracts transaction details automatically.
4. Review and verify the extracted transactions.
5. Run the subscription detection engine.
6. View detected recurring payments.
7. Review monthly and yearly subscription expenses.
8. Export extracted transactions as CSV.

## 6. Troubleshooting

- Ensure Python and Node.js are installed correctly.
- Activate the Python virtual environment before running the backend.
- Install Tesseract OCR and configure its executable path if OCR fails.
- Verify that frontend API requests point to the correct backend URL.
- Ensure the uploaded PDF is readable and supported.
- Check backend terminal logs for extraction or processing errors.

## 7. Development Notes

- Backend: Python, FastAPI
- Frontend: React, Vite
- PDF Processing: PyMuPDF
- OCR: Tesseract
- Data Processing: Pandas
- Subscription Detection: Pattern matching and merchant similarity analysis

The application runs locally during development and can subsequently be deployed to a cloud hosting platform.


## 5. Feature Demonstration

Provide step-by-step instructions for accessing and testing each of your two selected features.

### Feature 1: [Feature Name]
1. [Steps to access the feature.]
2. [Steps to test its functionality.]
3. [Expected outcome.]

### Feature 2: [Feature Name]
1. [Steps to access the feature.]
2. [Steps to test its functionality.]
3. [Expected outcome.]
