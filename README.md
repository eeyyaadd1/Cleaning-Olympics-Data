# 🏅 Olympics Data Cleaning Project
📌 Overview
This project demonstrates a complete data cleaning workflow using Python and Pandas. I transformed a raw dataset of historical Olympic results into a structured, analysis-ready format. The process involved handling complex string patterns, managing missing values, and optimizing data types.

🛠️ Data Cleaning Steps (Pipeline)
# I followed a structured checklist to ensure the data's integrity and usability:

### 1. Encoding & Data Loading: 
  Resolved character encoding issues (UTF-8) to ensure athlete names like Jean-François Blanchy are rendered correctly. Added low_memory=False to handle mixed-type columns efficiently.

### 2. Feature Engineering (Regex Extraction):

  Games Split: Used Regular Expressions to split the Games column into separate year and type (Summer/Winter) columns.

  Position Cleanup: Extracted numerical rankings from the Pos column while identifying "Tied" results.

### 3. Handling Mixed Types & Logic:

  Tied Flag: Created a boolean tied column to preserve information about shared rankings before converting positions to numeric.

  Non-numeric Handling: Converted non-numeric values (like DNS, DNF) in the position column to NaN to maintain mathematical consistency.

### 4. Missing Value FIX:

  Replaced NaN in medals with "No Medal".

  Filled missing team information with "Individual".

  Ensured the dataset is fully clean and ready for visualization without null value errors.

### 5. Schema Optimization:
  Renamed ambiguous columns (e.g., As to Name), dropped unnecessary columns, and reordered the dataset for better readability.
