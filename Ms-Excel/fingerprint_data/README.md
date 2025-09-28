# 📝 Fingerprint Data Attendance Analysis

This project automates the process of **employee attendance tracking** using biometric fingerprint logs.  
It extracts data from raw biometrics, maps them to employees, and generates an updated attendance sheet.

---

## 📌 Project Overview
- **Objective**: Convert raw fingerprint records into a structured monthly attendance sheet.  
- **Logic**:  
  - If an employee **clocks in and clocks out** (even multiple times in one day), it is counted as **1** for that day in the attendance sheet.  
  - The **total number of 1’s** is then summed for each employee to calculate the total days present in the month.  
  - If a new employee appears in the biometric data but does not exist in the attendance sheet, their name is automatically appended with `"Labourer"` as the default job description.  

---

## 📂 Files in This Project
1. **Biometrics Datasheet** → Raw fingerprint log data for employees.  
2. **May 2025 Attendance (Empty Sample)** → Template of an attendance sheet for May 2025 with structure but no records.  
3. **June 2025 Attendance (Analyzed)** → Processed sheet where raw biometric data is transformed into daily attendance (1’s) and monthly totals.  

---

## 🔧 Methodology
1. Import biometric data.  
2. Match fingerprint entries with employee names in the attendance sheet.  
3. Assign **1 per day** if there is at least one valid clock-in/out record (ignores multiple entries in the same day).  
4. Update totals for each employee.  
5. Append new employees if detected in biometrics but missing in attendance.  

---

## 📊 Output
- Clean attendance sheet with:  
  - **Daily presence marked as 1 or 0**  
  - **Total number of days worked per employee**  
  - **Automatically updated employee list if new staff are detected**  

---

## 🚀 Use Case
This project simplifies HR/Payroll operations by eliminating manual counting of daily clock-ins/outs, ensuring accuracy and efficiency in employee attendance management.
