# 🎓 KIIT University Student ERP & Academic Management System

[![Python 3.9+](https://img.shields.io/badge/Python-3.9%2B-blue.svg)](https://www.python.org/)
[![Framework: Django](https://img.shields.io/badge/Framework-Django%203.x-092E20.svg?logo=django&logoColor=white)](https://www.djangoproject.com/)
[![UI: AdminLTE 3](https://img.shields.io/badge/UI-AdminLTE%203-3c8dbc.svg)](https://adminlte.io/)
[![Frontend: Bootstrap 4](https://img.shields.io/badge/Frontend-Bootstrap%204-7952B3.svg?logo=bootstrap&logoColor=white)](https://getbootstrap.com/)
[![Database: SQLite / PostgreSQL](https://img.shields.io/badge/Database-SQLite%20%7C%20PostgreSQL-003B57.svg)](https://www.sqlite.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

An enterprise-grade academic management and Enterprise Resource Planning (ERP) web application developed for **Kalinga Institute of Industrial Technology (KIIT)**. The system provides unified role-based workflows for university administrators, academic faculty, and students, streamlining attendance monitoring, performance grading, leave processing, and institutional communications.

---

## 🏛️ System Architecture & Role-Based Workflows

```
                           ┌───────────────────────────┐
                           │      KIIT ERP System      │
                           └─────────────┬─────────────┘
                                         │
                 ┌───────────────────────┼───────────────────────┐
                 │                       │                       │
                 ▼                       ▼                       ▼
      ┌─────────────────────┐ ┌─────────────────────┐ ┌─────────────────────┐
      │  Administrator / HOD│ │   Faculty / Staff   │ │       Student       │
      ├─────────────────────┤ ├─────────────────────┤ ├─────────────────────┤
      │ • Overall Analytics │ │ • Subject Dashboard │ │ • Attendance View   │
      │ • Manage Staff      │ │ • Mark Attendance   │ │ • Academic Results  │
      │ • Manage Students   │ │ • Submit Results    │ │ • Apply for Leave   │
      │ • Courses & Subjects│ │ • Apply for Leave   │ │ • Send Feedback     │
      │ • Leave Approvals   │ │ • Student Feedback  │ │ • Profile Settings  │
      │ • System Logs       │ │ • Real-Time Stats   │ │ • Course Overview   │
      └─────────────────────┘ └─────────────────────┘ └─────────────────────┘
```

---

## ✨ Core Functionalities

### 1. 🛡️ Administrator / HOD Portal
* **Comprehensive Dashboard:** Real-time analytics displaying total active students, faculty count, registered courses, and departmental attendance trends.
* **Faculty & Student Management:** Full CRUD operations for student and staff records, including automated credential generation and profile image storage.
* **Curriculum Management:** Dynamic assignment of subjects, academic sessions, and course curricula across engineering disciplines.
* **Attendance Oversight:** Institution-wide attendance auditing per semester, branch, and subject.
* **Leave & Feedback Governance:** Formal review workflow for staff and student leave requests and grievance feedback submissions.

### 2. 👨‍🏫 Faculty / Staff Portal
* **Daily Attendance Recording:** Interactive multi-student roll-call interface with instant database updates.
* **Performance Grading:** Input and update internal examination marks and final grades with automated percentage calculation.
* **Leave Requests:** Digital leave application submission with status tracking (Pending, Approved, Rejected).
* **Direct Feedback Channel:** Submit departmental suggestions and academic reports directly to the HOD.

### 3. 👨‍🎓 Student Portal
* **Personalized Dashboard:** Visual progress metrics tracking attendance percentages across enrolled subjects with threshold alerts.
* **Academic Report Card:** Semester-wise examination score sheets and subject grade distributions.
* **Digital Leave Application:** Submit medical and personal absence requests directly to faculty.
* **Institutional Feedback:** Secure mechanism to voice feedback regarding coursework and facilities.

---

## 📸 Interface Screenshots

| Administrator Dashboard | Faculty Portal | Student Portal |
| :---: | :---: | :---: |
| <img src="ss/admin5.png" width="300" alt="Admin Dashboard"/> | <img src="ss/staff1.png" width="300" alt="Staff Dashboard"/> | <img src="ss/student1.png" width="300" alt="Student Dashboard"/> |
| <img src="ss/admin2.png" width="300" alt="Admin Courses"/> | <img src="ss/staff2.png" width="300" alt="Attendance Management"/> | <img src="ss/student2.png" width="300" alt="Attendance Summary"/> |
| <img src="ss/admin3.png" width="300" alt="Admin Staff Management"/> | <img src="ss/staff3.png" width="300" alt="Result Entry"/> | <img src="ss/student3.png" width="300" alt="Student Grades"/> |

---

## 🛠️ Technology Stack

* **Backend:** Python 3.9+, Django Web Framework (ORM, Authentication, Middleware, Form Validation)
* **Frontend:** AdminLTE 3, Bootstrap 4, HTML5, CSS3, JavaScript (DOM Manipulation, Chart.js)
* **Database:** SQLite (default for development), PostgreSQL-compatible ORM configuration
* **Security:** Django CSRF Protection, Password Hashing (`PBKDF2SHA256`), Role-Based Permissions (`CustomUser` model)

---

## 🚀 Quickstart & Setup Guide

### 1. Clone the Repository
```bash
git clone https://github.com/23051921/KIIT_ERP_FINAL.git
cd KIIT_ERP_FINAL
```

### 2. Create and Activate Virtual Environment
```bash
# On Windows
python -m venv venv
.\venv\Scripts\activate

# On Linux / macOS
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Required Dependencies
```bash
pip install -r requirements.txt
```

### 4. Apply Database Migrations
```bash
python manage.py makemigrations
python manage.py migrate
```

### 5. Launch the Development Server
```bash
python manage.py runserver
```

Open [http://127.0.0.1:8000](http://127.0.0.1:8000) in your web browser.

---

## 📄 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
