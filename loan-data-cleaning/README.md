This project focuses on cleaning and preparing a bank loan dataset containing 5,000 customer records. The goal was to take a raw CSV file and turn it into a structured, reliable dataset that can be used for analysis or modeling. The work includes checking data quality, fixing inconsistencies, handling missing values, and exporting a clean version of the file.
click on the link to view this project on google colab:

Dataset
The dataset includes customer demographic and financial information such as:

Age

Experience

Income

Family size

Credit card spending

Education level

Mortgage amount

Account and loan indicators

What I Did
1. Loaded and inspected the data
I used pandas to read the CSV file and reviewed the structure using:

df.head()

df.info()

df.describe()

df.isnull().sum()

This helped me understand data types, missing values, and any potential issues.

2. Cleaned data types
One column (CCAvg) was stored as text instead of numeric. I identified this early and prepared it for conversion during the cleaning process.

3. Handled missing values
Numeric columns were filled using the median

Categorical columns were filled using the mode

This approach keeps the data consistent without distorting distributions.

4. Checked for duplicates
I verified that the dataset contained no duplicate rows, so no removal was needed.

5. Standardized categorical text
For object‑type columns, I:

Stripped extra spaces

Converted text to lowercase

This prevents issues where similar values are treated as different categories.

6. Exported the cleaned dataset
The final cleaned file was saved as bank_loan_cleaned.csv for future use.

Tools Used
Python

pandas

numpy

Google Colab

Key Takeaways
This project strengthened my experience with:

Data quality checks

Cleaning and preparing structured datasets

Handling mixed data types

Writing clear, repeatable preprocessing steps
