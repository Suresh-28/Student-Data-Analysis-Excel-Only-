# 📊 Student Data Analysis (Excel Only)

This repository contains **student performance data analysis** done entirely in **Microsoft Excel**.  
No Python or external programming tools were used.

## 📂 Contents
- `excel/Student Data for Pivot Table.xlsx` → Main Excel file with raw data and analysis.
- `Formulas.md` → Documentation of formulas and functions used.
- `README.md` → Project overview.

## 📌 Features
- Student performance dataset.
- Pivot tables for summarizing:
  - Average marks per subject.
  - Top scorers.
  - Count of students by grade/class.
- Conditional formatting for quick insights.
- Reusable formulas for dynamic calculations.

## 🚀 Usage
1. Download the Excel file from `excel/`.
2. Open it in **Microsoft Excel** (or Google Sheets).
3. Explore pivot tables and formulas applied.
4. You can add more data and analysis will auto-update.

## 🛠️ Tools Used
- Microsoft Excel (Pivot Tables, Formulas, Charts)
- Conditional Formatting



# 📘 Excel Formulas Used

## 1. Basic Statistics
- **Total Marks** → `=SUM(B2:F2)`
- **Average Marks** → `=AVERAGE(B2:F2)`
- **Highest Mark** → `=MAX(B2:F2)`
- **Lowest Mark** → `=MIN(B2:F2)`

## 2. Conditional Analysis
- **Pass/Fail** → `=IF(AVERAGE(B2:F2)>=40,"Pass","Fail")`
- **Grade Assignment** → 
  ```excel
  =IF(AVERAGE(B2:F2)>=90,"A+",
     IF(AVERAGE(B2:F2)>=75,"A",
     IF(AVERAGE(B2:F2)>=60,"B",
     IF(AVERAGE(B2:F2)>=50,"C","F"))))
3. Lookup

Student Name Lookup by ID → =VLOOKUP(101,$A$2:$G$50,2,FALSE)

4. Pivot Table Insights

Average marks by subject.

Number of students per grade.

Top 5 students by marks.

Distribution of pass/fail.

5. Conditional Formatting

Highlight students scoring above 90 in green.

Highlight students failing in red.
