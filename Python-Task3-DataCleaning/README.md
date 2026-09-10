
## Project Overview
This project focuses on cleaning and preprocessing a deliberately messy Titanic dataset using Python and Pandas.

The main objective is to identify and fix common data quality issues such as missing values, duplicate records, inconsistent formatting, incorrect data types, and outliers.

## Dataset
The project uses the Titanic dataset containing passenger information such as age, gender, passenger class, fare, and survival status.

## Technologies Used
- Python
- Pandas
- NumPy
- Jupyter Notebook

## Data Quality Checks
The dataset was analyzed for:
- Missing values
- Duplicate records
- Incorrect data types
- Inconsistent categorical values
- Invalid numeric values
- Range anomalies and outliers

## Data Cleaning Performed

### 1. Missing Value Handling
Missing values were identified and handled using appropriate techniques.

- Age values were converted to numeric and missing values were filled using the median.
- Embarked missing values were handled using the most appropriate categorical value.
- Fare values were converted to numeric and missing values were filled using the median.

### 2. Duplicate Removal
Duplicate rows were identified and removed to ensure that each record was unique.

### 3. Standardization
Inconsistent categorical values were standardized.

For example:
- `male`, `MALE`, `M`, etc. were standardized to `Male`.
- `female`, `F`, etc. were standardized to `Female`.
- Embarked values were standardized to consistent categories.

### 4. Data Type Correction
Columns were converted to appropriate data types.

- PassengerId → Integer
- Survived → Integer
- Pclass → Integer
- Age → Numeric
- SibSp → Integer
- Parch → Integer
- Fare → Numeric
- Sex → String
- Embarked → String

### 5. Outlier Detection
The Interquartile Range (IQR) method was used to identify potential outliers in numerical columns.

Outliers were reviewed and handled appropriately without unnecessarily removing valid passenger records.

## Before vs After

After cleaning:
- Missing values were removed or appropriately handled.
- Duplicate records were removed.
- Categorical values were standardized.
- Numerical columns were converted to correct data types.
- Invalid values and anomalies were addressed.

## Output

The cleaned dataset is saved as:

`Titanic_Cleaned.csv`

## Project Files

- `Task_3_Data_Cleaning_Titanic.ipynb` - Complete data cleaning and preprocessing notebook.
- `Titanic_Cleaned.csv` - Final cleaned dataset.

## Conclusion
The project demonstrates a complete data-cleaning workflow using Python and Pandas.

The cleaned dataset is more consistent, reliable, and ready for further analysis or machine learning applications.
