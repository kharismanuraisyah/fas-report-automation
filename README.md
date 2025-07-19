# 🚚 FAS Report Automation

This is a Google Colab project that automates the generation of daily **FAS (First Attempt Success)** reports for last-mile delivery. The notebook performs data cleaning, grouping by region, pivot analysis, making file .xlsx and finally uploads the results to a Google Sheet.

---

## 📌 Overview

- Reads raw CSV data from Metabase export
- Filters and groups data by regions:
  - Intim
  - Northern
  - Southern
  - etc
- Exports Excel files for each region
- Creates a combined pivot table for "Hit" and "Miss"
- Uploads the pivot result to a shared Google Sheet

---

## 🧰 Dependencies

- `pandas`
- `openpyxl`
- `gspread`
- `google-auth` (via service account)

---

## 🚀 How to Use

1. Upload your own `rawdata.csv` data
2. Upload your Google Sheets service account JSON (not included)
3. Run the notebook step by step
4. The script will:
   - Create Excel files
   - Generate pivot table
   - Update your Google Sheet

---

## 🔐 Note on Credentials

This notebook requires a Google service account credential to update Google Sheets.  
**The credential is not included** in this repository.  
Please upload your own `.json` file when running the notebook.

> 📌 The notebook is cleaned and safe to showcase publicly.

---

## 💡 Sample Output

- Excel: `fas_intim.xlsx`, `fas_northern.xlsx`, `fas_southern.xlsx`, etc
- Google Sheet with pivot table updated daily

---

## 🙋‍♀️ Author

Kharisma Nur’aisyah  
[LinkedIn](https://www.linkedin.com/in/kharismanuraisyah/)
