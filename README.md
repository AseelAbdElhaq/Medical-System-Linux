# 🏥 MyPharmacy – Linux Shell Script Project

## 📌 Project Overview
**MyPharmacy** is a Linux shell script project developed as part of **COMP311 (Linux OS Lab) / COMP438 (UNIX OS)**.  
It is a **pharmacy management system** that enables pharmacists to manage drug records, update stock, and process prescriptions efficiently through a command-line interface.  

The project demonstrates:
- Modular Bash scripting
- File handling in Linux/UNIX
- Input validation and error checking
- Real-world pharmacy operations in a simplified system

---

## ⚙️ Features
### 1. Add Drug
- Requires a **unique 4-digit ID** (validated, must not repeat).  
- Scientific name (letters, dashes, backslashes allowed).  
- Trade name (letters, digits, dashes, backslashes allowed, cannot start with a digit).  
- Price (digits only).  
- Manufacturing Date (`dd/mm/yyyy` format).  
- Expiration Date (auto-generated, +547 days from manufacturing date).  
- Quantity (digits only).  

### 2. Modify Drug
- **Delete Drug** → Remove by exact ID.  
- **Update Drug Info** → Modify fields except ID & expiration date.  
- Expiration updates automatically if manufacturing date is changed.  

### 3. Search Drugs
- **By ID** → Show details if exists.  
- **By Scientific/Trade Name** → Full or partial match, sorted by trade name.  
- **By Expiration Date** → Display all drugs in descending order.  
- **By Quantity** → Display all drugs in ascending order.  

### 4. Prescription
- Search drug by ID or Trade Name.  
- Dispense quantity validated against stock.  
- Deduct stock after successful dispense.  
- Repeat dispensing until `stop` is entered.  
- Display **total cost** of all dispensed drugs.  

---

## ▶️ How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/username/myPharmacy.git
   cd myPharmacy
   chmod +x *.sh
   ./myPharmacy.sh

   ---

## 🛠️ Technologies Used

Bash (Shell Scripting)

Linux/UNIX Environment

Text-based Database (drugs.txt)


