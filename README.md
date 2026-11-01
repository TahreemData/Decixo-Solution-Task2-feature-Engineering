# Decixo-Solution-Task2-feature-Engineering
# Hotel Booking Data Cleaning & Feature Engineering

## Project Overview
This project focuses on data cleaning and feature engineering using the **Hotel Booking Demand Dataset**. The main objective is to improve data quality and prepare the dataset for further data analysis and machine learning using Python.

## Objectives
- Identify and handle missing values.
- Detect and remove duplicate records.
- Detect and handle outliers.
- Correct data types.
- Perform categorical encoding.
- Apply numerical standardization.
- Create meaningful features.
- Compare data statistics before and after cleaning.

## Dataset Description
The dataset contains hotel booking information, including:

- Hotel type
- Booking cancellation
- Lead time
- Arrival dates
- Number of guests
- Country
- Market segment
- Agent and company
- Average Daily Rate (ADR)
- Special requests
- Reservation status

## Tools & Technologies
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Data Cleaning Process

### 1. Missing Values
Missing values were identified in four columns:

| Column | Missing Values |
|---|---:|
| Children | 4 |
| Country | 488 |
| Agent | 16,340 |
| Company | 112,593 |

**Treatment:**
- Children: Median imputation.
- Country: Replaced with Unknown.
- Agent: Replaced with 0.
- Company: Replaced with 0.

### 2. Duplicate Removal
A total of **31,994 duplicate records** were identified and removed using Pandas.

### 3. Outlier Detection
The Interquartile Range (IQR) method was used to identify outliers in the ADR column. Extreme values were capped using calculated limits.

### 4. Data Type Conversion
Date columns were converted into datetime format, and numerical columns were checked for appropriate data types.

## Feature Engineering
Seven new features were created:

1. Total Guests
2. Total Nights
3. Is Family
4. Has Special Requests
5. Has Weekend Stay
6. Booking Month
7. Estimated Room Revenue

## Data Transformation

- **One-Hot Encoding:** Used to convert categorical variables into numerical format.
- **StandardScaler:** Used to standardize numerical features.
- **Preprocessing Pipeline:** Scikit-learn was used to demonstrate automated preprocessing.

## Project Structure

```text
Hotel-Booking-Data-Cleaning/
│
├── hotel_bookings.csv
├── Task_2_Data_Cleaning.ipynb
├── Hotel_Booking_Cleaned.csv
├── Hotel_Booking_Encoded_Standardized.csv
├── README.md
│
└── Executive_Summary/
```

## Key Results

- Identified and treated missing values.
- Removed 31,994 duplicate records.
- Detected and handled outliers.
- Created seven meaningful features.
- Encoded categorical variables.
- Standardized numerical features.
- Prepared datasets for further analysis.

## Conclusion

This project demonstrates the importance of data cleaning and feature engineering in the data analytics process. The preprocessing techniques improved data consistency and prepared the Hotel Booking Demand dataset for further analysis and machine learning applications.

## Author
**Tahreem M. Nadeem**

**Project:** Task 2 – Data Cleaning & Feature Engineering

**Organization:** Devixo Solutions
