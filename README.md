# 🎓 Student Enrollment Form
<img width="1215" height="510" alt="image" src="https://github.com/user-attachments/assets/308bd314-42b1-4618-a38c-9a52a814c60a" />
<img width="754" height="365" alt="image" src="https://github.com/user-attachments/assets/dd9cd44c-e456-4bd7-8ea1-364897f02335" />


A responsive **Student Enrollment Management Web Application** built using **HTML, CSS, Bootstrap, JavaScript, jQuery, and JsonPowerDB (JPDB)**.

This project allows users to **save, update, reset, and fetch student records** dynamically using JsonPowerDB as the backend database.

---

## ✨ Project Preview

### Features Included
✅ Responsive modern UI  
✅ Student record creation  
✅ Auto fetch existing student data using Roll Number  
✅ Update student details  
✅ Reset form functionality  
✅ Field validation (No empty fields allowed)  
✅ JsonPowerDB database integration  
✅ Primary key based record checking  
✅ Mobile-friendly design  

---
const connToken = "90935204|-31949243650444739|90958775";

## 📌 Problem Statement

Create a form-based Student Enrollment System where:

- User enters **Roll Number (Primary Key)**.
- If the Roll Number does **not exist**, user can enter student details and save them.
- If the Roll Number **already exists**, existing data is automatically fetched.
- User can then update the existing record.
- Reset button clears the form and restores initial state.

---

## 🛠 Tech Stack

### Frontend
- HTML5
- CSS3
- Bootstrap 5
- JavaScript
- jQuery

### Backend / Database
- JsonPowerDB (JPDB)

---
const dbName = "SCHOOL-DB";
const relName = "STUDENT-TABLE";
const baseUrl = "http://api.login2explore.com:5577";
const apiEndPoint = "/api/iml";

## 🗄 Database Details

| Property | Value |
|--------|------|
| Database Name | SCHOOL-DB |
| Relation Name | STUDENT-TABLE |
| Primary Key | Roll-No |

---

## 📋 Form Fields

- Roll No *(Primary Key)*
- Full Name
- Class
- Birth Date
- Address
- Enrollment Date

---

## 🚀 Functional Workflow

### Initial State
- Only **Roll No** field is enabled
- All other fields are disabled
- Save, Update, Reset buttons are disabled

---

### New Record Flow
1. Enter Roll No
2. System checks database
3. If record doesn't exist:
   - Enable input fields
   - Enable Save + Reset buttons
4. Fill details
5. Click Save
6. Record stored in JsonPowerDB

---

### Existing Record Flow
1. Enter Roll No
2. System checks database
3. If record exists:
   - Fetch existing data
   - Auto-fill form
   - Disable Roll No
   - Enable Update + Reset buttons
4. Modify details
5. Click Update

---

## 📂 Project Structure

```bash
Student-Enrollment-Form/
│
├── index.html
├── README.md
