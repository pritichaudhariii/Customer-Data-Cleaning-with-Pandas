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

## 🔄 Cleaning Summary

- Removed duplicates and unnecessary columns
- Cleaned last names by stripping extra characters
- Standardized phone numbers into XXX-XXX-XXXX format and dropped invalid ones
- Split full address into Street, City, and Zip
- Normalized values for Paying Customer and Do_Not_Contact (Y/N)
- Replaced inconsistent missing values with blanks
- Dropped records flagged as Do_Not_Contact
- Reset index and exported cleaned dataset to Excel
