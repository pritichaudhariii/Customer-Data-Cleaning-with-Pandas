# Customer Data Cleaning with Pandas

# 📌 Project Overview

This project demonstrates how to clean and standardize a messy customer contact list using **Python (Pandas)**.  
The dataset originally contained issues such as inconsistent phone number formats, combined address fields, missing values, and customers flagged as `Do_Not_Contact`.  

The goal was to transform the raw Excel file into a clean, analysis-ready dataset and export it in both Excel and CSV formats.

🛠️ Tech Stack
- **Python 3**
- **Pandas** for data cleaning and transformation
- **OpenPyXL** for Excel file handling
- **Jupyter Notebook** for interactive processing

## 🔄 Cleaning Steps
1. Loaded raw Excel data into a Pandas DataFrame.  
2. Standardized phone numbers into the format `XXX-XXX-XXXX`.  
3. Split `Address` into `Street`, `City`, and `Zip`.  
4. Handled missing values by replacing with `None`.  
5. Removed customers flagged as `Do_Not_Contact`.  
6. Dropped unnecessary columns after splitting.  
7. Exported the cleaned dataset to `.xlsx`.

📊 Example Results

Before Cleaning:

Phone_Number     Address                          Do_Not_Contact
123/543-2345     980 Paper Avenue, Pennsylvania   Y
(876)678|3469    25th Main Street, New York       N
N/a              123 Middle Earth                 NaN


After Cleaning:

Phone_Number     Street               City            Zip      Do_Not_Contact
123-543-2345     980 Paper Avenue     Pennsylvania    18503    Y
876-678-3469     25th Main Street     New York        NaN      N
NaN              123 Middle Earth     NaN             NaN      None
