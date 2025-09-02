# HealthyLife — OOP Healthcare Mini-System (Python)

**Goal:** Demonstrate clean OOP design and extensibility in a healthcare domain using design patterns.

### What it does
- Models **Patient, Doctor, Nurse, Appointment, MedicalHistory**
- Supports **insurance plans** (Dental, Eyecare, Medical, Wellness) via **Abstract Factory**
- Switchable **billing rules** (Standard, Discount, Co-Pay, Telehealth) via **Strategy**
- **Observer** pattern to notify subscribers when Doctor/Nurse availability, specialty, or fees change
- Demo flow: create patient & staff → book appointments (incl. telehealth) → complete appointment → print invoice & history

### Tech
- Python (Jupyter Notebook)

### Run
1. Open `Healthcare_oop.ipynb` in Jupyter.
2. Run all cells (or scroll to the `if __name__ == "__main__":` section and run).

### Highlights
- **Abstract Factory:** `InsuranceFactory` → `Dental/Eyecare/Medical/WellnessCoverage`
- **Strategy:** `InvoiceStrategy` → `StandardInvoice`, `DiscountInvoice`, `CoPayInvoice`, `TelehealthInvoice`
- **Observer:** `Doctor`/`Nurse` maintaining observers and notifying on changes

