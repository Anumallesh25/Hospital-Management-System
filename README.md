# Hospital-Management-System
A Hospital Management System is software designed to manage all aspects of hospital operations, including patient records, appointments, billing, staff management, and inventory. It streamlines workflows, improves efficiency, ensures data accuracy, and enhances the overall patient care experience.
Hospital Management System - DBMS Mini Project

This project is a **Hospital Management System** built as a **Database Management System (DBMS) mini project**. It is designed to manage hospital operations such as patient information, doctor records, appointments, billing, and more using a relational database.

Features

- Add, update, delete, and search **patient records**
- Manage **doctor profiles** and specializations
- Schedule and track **appointments**
- Maintain **medical records** and treatment history
- Generate and manage **bills and payments**
- Track **hospital rooms** and availability
- Admin panel for hospital staff to manage data
- Relational schema with proper foreign keys and normalization


Technologies Used

- **Frontend / UI**: C++, Python (Tkinter), Java, or Web (HTML/CSS/JS) – based on implementation
- **Backend / Logic**: SQL (Structured Query Language)
- **Database**: MySQL / SQLite / PostgreSQL (choose based on setup)
- **Tools**: MySQL Workbench, XAMPP, phpMyAdmin, or terminal-based clients


Database Schema

- `Patients(patient_id, name, age, gender, contact, address)`
- `Doctors(doctor_id, name, specialization, contact)`
- `Appointments(appointment_id, patient_id, doctor_id, date, time)`
- `MedicalRecords(record_id, patient_id, diagnosis, treatment, notes)`
- `Billing(bill_id, patient_id, total_amount, date, status)`
- `Rooms(room_id, type, availability)`

All tables are linked via primary and foreign keys to ensure data integrity and consistency.

Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/hospital-management-dbms.git
   cd hospital-management-dbms
Setup the database

Import hospital_db.sql into your MySQL or SQLite server:

sql
Copy
Edit
SOURCE hospital_db.sql;
Run the application

Use CLI, GUI tool, or front-end script depending on your interface

Sample SQL Queries
sql
Copy
Edit
-- View all patients
SELECT * FROM Patients;

-- Get appointments for a specific doctor
SELECT * FROM Appointments WHERE doctor_id = 101;

-- Calculate total billing for a patient
SELECT SUM(total_amount) FROM Billing WHERE patient_id = 1001;

Future Improvements
Add user authentication (admin, doctor, receptionist)
Include pharmacy and lab modules
Generate PDF reports for billing and diagnosis
Web-based or mobile-friendly UI




