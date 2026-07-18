# CareSync Database Design

## Tables

- Users
- Departments
- Doctors
- Patients
- Appointments
- Prescriptions

## 1. Users

| Column | Type | Description |
|---------|------|-------------|
| id | UUID/INT | Primary Key |
| name | VARCHAR | User Full Name |
| email | VARCHAR | Unique Email |
| password_hash | VARCHAR | Encrypted Password |
| role | ENUM | ADMIN, DOCTOR, PATIENT |
| phone | VARCHAR | Contact Number |
| is_active | BOOLEAN | Account Status |
| created_at | TIMESTAMP | Creation Time |
| updated_at | TIMESTAMP | Last Update |

---

## 2. Departments

| Column | Type | Description |
|---------|------|-------------|
| id | INT | Primary Key |
| name | VARCHAR | Department Name |
| description | TEXT | Description |
| floor | INT | Hospital Floor |
| created_at | TIMESTAMP | Creation Time |