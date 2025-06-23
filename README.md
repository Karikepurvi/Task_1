Hi! This is my submission for Task 1 of the Data Analyst Internship – focused on data cleaning and preprocessing. The dataset I worked with is called `marketing_campaign.csv`, which contains customer details like education level, income, and marketing responses.
Here’s a summary of what I did:

- **Checked for missing values** using `.isnull().sum()`  
  - Filled missing values in the `Income` column using the average income  
  - Dropped one row where the `Dt_Customer` (customer joining date) was missing

- **Removed duplicate rows** using `.drop_duplicates()`  
  - This helped ensure clean and consistent data

- **Converted the `Dt_Customer` column** to a proper `datetime` format (`dd-mm-yyyy`)  
  - This makes date-based analysis easier in the future

- **Standardized and cleaned up the column names**  
  - Changed all column headers to lowercase and replaced spaces with underscores  
  - For example: `Year_Birth` → `year_birth`

- **Checked and fixed data types**  
  - Made sure columns like `year_birth` are integers

- **Cleaned text fields like `Education`** by applying formatting functions (title case, strip spaces)

 Cleaning data is one of the most important steps before analysis. Dirty data leads to wrong conclusions. Through this task, I learned how to systematically identify and fix common issues like:
- Missing values
- Duplicate records
- Inconsistent formats
- Messy column names
  
  Tools used 
- Python
- Pandas
- Google Colab
  
