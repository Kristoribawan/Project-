# Student Document Request Monitoring System

**PHINMA Cagayan de Oro College**

A console-based academic document request and monitoring system written in Python.  
This application streamlines the request process for official school documents, enabling students to place requests online while providing administrators with a central management console to track, update, and manage student accounts and document records.

---

## System Overview

The system operates using a dual-role structure (**Admin** and **Student**):

* **Students** can create accounts, log in, view standard document fees, submit new requests, and check the real-time status of their applications.
* **Administrators** can review all incoming requests, update fulfillment statuses (*Pending*, *Processing*, *Ready for Claiming*, *Completed*), view registered student accounts, and access transaction logs.

---

## Core Features

### 1. Student Portal
* **Account Registration:** Create student accounts with built-in validation for duplicate usernames and unique School IDs.
* **Document Request Catalog:** Interactive price list for standard institutional documents.
* **Request Tracking:** View current active requests and past request history.

### 2. Admin Portal
* **Request Management:** Display all submitted requests with complete student and document details.
* **Status Updates:** Update request fulfillment states interactively.
* **Student Registry:** View all registered student accounts and credentials.
* **Transaction Records:** Monitor complete document request logs.

---

## Document Price List

Document Type | Standard Price
--- | ---
Transcript of Records | ₱150
Certificate of Enrollment | ₱100
Certificate of Good Moral Character | ₱100
Certificate of Graduation | ₱150
Clearance | ₱50
Certificate of Completion | ₱100
Diploma | ₱200
Certificate of Transfer Credentials | ₱150
Certificate of Enrollment History | ₱100
Certificate of Honorable Dismissal | ₱150

---

## Default Credentials

### Admin Login
* **Username:** `admin`
* **Password:** `admin123`

### Pre-loaded Student Account
Username | Password | School ID | Gender
--- | --- | --- | ---
jay | jay123 | 126519120056 | Male

---

## How to Run

1. Ensure **Python 3** is installed on your computer.
2. Save the source code into a file named `main.py` (or `document_system.py`).
3. Open your terminal or command prompt and execute:

```bash
python main.py

or

python3 main.py

Technical Highlights

1. Data Structures: Uses Python dictionaries (students, document_requests, documents) for efficient lookup and state management.
2. Auto-Incrementing Tracking Numbers: Generates unique tracking IDs starting at 1001 for every submitted document request.
3. Input Validation: Prevents blank inputs, duplicate usernames, duplicate School IDs, invalid genders, and mismatched passwords during account creation.

System Limitations & Future Scope
1. In-Memory Storage: Data resets when the application is closed (no external database or file persistence).
2. CLI Interface: Text-based command-line interface.
3. Planned Improvements: Integration with SQLite/MySQL, PDF receipt generation, and a Graphical User Interface (GUI).

Author
Developed as a student project for PHINMA Cagayan de Oro College.
