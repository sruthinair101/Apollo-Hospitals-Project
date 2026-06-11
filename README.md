# 🏥 Apollo Hospitals – Healthcare Analytics Dashboard (Power BI)

> **"Touching Lives"** — An end-to-end Power BI dashboard built on the Apollo Healthcare dataset to analyze patient records, billing, bed utilization, doctor performance, and diagnosis trends.

---

## 📌 Project Overview

This Power BI report transforms raw hospital data into actionable insights across six analytical focus areas. It enables hospital administrators and healthcare analysts to monitor operations, identify bottlenecks, and make data-driven decisions.

**Tool:** Microsoft Power BI Desktop  
**Dataset:** Apollo Healthcare Dataset (`Apollo-Healtcare-Dataset.xlsx`)  
**Date Range:** December 2022 – March 2024  
**Total Billing Volume:** ₹190M+

---

## 📂 Dataset Schema

The dataset (`Sheet1`) contains the following fields:

| Column | Description |
|---|---|
| `Patient_ID` | Unique identifier for each patient |
| `Admit_Date` | Date of hospital admission |
| `Discharge_Date` | Date of discharge |
| `Diagnosis` | Medical diagnosis (Viral Infection, Flu, Malaria, etc.) |
| `Bed_Occupancy` | Ward type — Private, General, ICU |
| `Test` | Diagnostic test performed (MRI, CT Scan, Blood Test, etc.) |
| `Doctor` | Treating doctor's name |
| `Followup Date` | Scheduled follow-up date post-discharge |
| `Feedback` | Patient feedback score for the doctor |
| `Billing Amount` | Total bill charged to the patient (₹) |
| `Health Insurance Amount` | Insurance coverage amount (₹) |

---

## 📊 Dashboard Sections & Business Questions

### 1. 🧍 Patient Information (by Patient ID)
**Question:** What are the complete details of a specific patient's hospital visit?

- Lookup individual patient records using the **Patient ID slicer**
- Displays: Admit Date, Discharge Date, Follow-up Date
- Enables case-by-case review for administrative or clinical purposes

---

### 2. 💳 Billing Information
**Question:** What is the total billing amount across all patients, and how does it trend over time?

- KPI card showing **Total Billing Amount: ₹190M**
- Date range filter (Admit Date slider) to scope billing by period
- Line chart: **Billing Amount vs. Health Insurance Amount** over time
- Reveals the gap between what patients are billed vs. what insurance covers

---

### 3. 🛏️ Bed Occupancy Breakdown
**Question:** How are hospital beds distributed across ward types?

- Bar chart comparing occupancy across:
  - **Private:** 3.6K
  - **General:** 2.4K
  - **ICU:** 1.2K
- Helps identify overutilized or underutilized wards
- Supports capacity planning and resource allocation decisions

---

### 4. ⭐ Overall Feedback for Doctors
**Question:** How do patients rate each doctor, and is feedback evenly distributed?

- Donut chart showing **Feedback Volume per Doctor**
- Doctors covered: Jay Sinha, Jaya Yaadav, Mark Joy, Naresh Goyenka, Niki Sharma, Ravi D, Tejas Saxena
- Each doctor has ~1.02K feedback entries — useful for detecting rating patterns or response bias

---

### 5. 🔬 Diagnosis-wise Statistics
**Question:** Which diagnoses are most prevalent in the patient population?

- Horizontal bar chart ranking diagnoses by patient count:
  - Viral Infection: **2.00K**
  - Flu: **1.72K**
  - Malaria: **1.43K**
  - Typhoid: **1.15K**
  - Pneumonia: **0.57K**
  - Fracture: **0.29K**
- Supports clinical resource planning and disease surveillance

---

### 6. 📈 Billing vs. Insurance Stats
**Question:** How does total billing compare to health insurance coverage over time?

- Dual-line area chart tracking both metrics across the date range
- Highlights out-of-pocket exposure for patients
- Insurance coverage appears consistently lower than billing — quantifies the coverage gap

---

## 🗂️ File Structure

```
📁 Apollo-Healthcare-Dashboard/
├── 📊 Apollo Dataset.pbix             # Power BI report file
├── 📄 Apollo-Healtcare-Dataset.xlsx  # Source dataset
└── 📝 README.md                       # Project documentation
```


## 🔍 Key Insights

- **Viral Infection** is the most common diagnosis, accounting for nearly twice the cases of Fracture
- **Private ward** has the highest bed occupancy, suggesting demand for premium care
- **Insurance consistently covers less than the billing amount** — the gap widens at higher billing values
- **Doctor feedback is uniformly distributed** (~1.02K per doctor), which may indicate a data collection artifact worth investigating rather than genuine parity

---

## 👤 Author

Built as part of a healthcare data analytics project using Power BI.  
Project By Shruti Nair
