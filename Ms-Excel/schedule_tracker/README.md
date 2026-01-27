# 🗓️ Employee Work Schedule Tracker

This project is a **dynamic Excel-based employee work scheduling tool** that automatically generates and updates a monthly work schedule based on a selected start date.

It is designed to simplify shift planning while ensuring **fair and complete shift allocation** across all employees.

---

## 📌 Project Overview

**Objective:**  
Create a flexible monthly work schedule that automatically adjusts dates, weekdays, and headings when the month or year is changed.

**Key Features:**
- Dynamic date and weekday generation
- Automatic heading update based on selected month and year
- Shift allocation validation to ensure no shift is left unassigned
- Clear shift descriptions for easy interpretation

---

## 📂 Files in This Project
- **Final Work Schedule Workbook** → The completed Excel file containing the dynamic scheduling system.
- **Screenshot (Data folder)** → Visual reference showing the final schedule output and layout.

---

## 🧠 Logic & Design

### Date & Header Automation
- A **Start Date** cell controls the entire schedule.
- When the start date is changed:
  - The **month and year heading** updates automatically  
    *(e.g., “Monthly Work Schedule for January 2026”)*.
  - The calendar dates and corresponding weekdays adjust accordingly.
  - The schedule dynamically aligns day numbers with correct weekdays  
    *(e.g., Thursday = 1, Saturday = 31 for January 2026)*.

---

### Shift Definitions
The schedule uses coded shift labels for clarity:
- **M** → Morning Shift  
- **A** → Afternoon Shift  
- **N** → Night Shift  

A dedicated shift description range explains each code.

---

### Shift Distribution Validation
- The system checks daily shift assignments to ensure:
  - Every shift (Morning, Afternoon, Night) is assigned.
  - No shift is left unattended due to uneven distribution.
- This promotes **fair workload sharing** among employees.

---

## 📊 Output
- A clean, monthly employee schedule with:
  - Automatically generated dates and weekdays
  - Clearly assigned shifts per employee
  - Dynamic month/year heading
  - Balanced shift coverage across all days

---

## 🚀 Use Case
This tool is ideal for **HR teams, operations managers, and supervisors** who need a reliable, reusable scheduling solution that minimizes manual errors and ensures fair shift allocation.

It can be reused for any month or year by simply changing the start date.
