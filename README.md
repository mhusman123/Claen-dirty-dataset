Project Report: Dirty Cafe Sales Data Cleaning & Analysis

Project Overview
This project involved cleaning and analyzing a messy transactional dataset from a fictional cafe business. The original data included customer transactions, item quantities, prices, payment methods, and locations — but it had numerous issues such as missing values, incorrect calculations, inconsistent formatting, and more.
Objectives
•	Clean and standardize the dataset
•	Handle missing and inconsistent values
•	Perform feature engineering
•	Scale numerical features
•	Visualize cleaned data for better business insights
Tools Used
•	Python (pandas, NumPy, matplotlib, seaborn, scikit-learn)
•	Jupyter Notebook
•	CSV Dataset (dirty_cafe_sales.csv)
Data Cleaning Steps
1.	Column Standardization
o	Converted all column names to lowercase for consistency.
2.	Null Value Handling
o	Filled missing item, location, and payment method values with 'Unknown'.
o	Filled quantity, price per unit, and total spent with median/mean values.
o	Forward-filled missing transaction date entries.
3.	Duplicate Removal
o	Removed duplicate records from the dataset.
4.	Text Formatting
o	Stripped extra spaces and standardized case formatting using .str.strip().str.title().
5.	Data Type Conversion
o	Converted transaction date to datetime.
o	Converted quantity to integer type.
6.	Feature Engineering
o	Recalculated total spent by multiplying quantity and price per unit.
o	Extracted month and day of week from the transaction date.
7.	Feature Scaling
o	Applied Min-Max Scaling to price per unit and total spent.
8.	Final Validation
o	Rechecked for remaining nulls, data types, and duplicate rows.
o	Ensured total spent values are logically consistent after recalculation.
Visualization
•	A histogram plot of total spent was generated after cleaning to visualize the distribution of spending behavior.
Results
•	Successfully cleaned and transformed 10,000+ messy records.
•	Created new features for better analysis.
•	Ensured dataset was 100% ready for analysis and modeling.
•	Exported the cleaned dataset as cleaned_cafe_sales.csv.
Deliverables
•	Cleaned dataset (.csv)
•	Python notebook with full cleaning process
•	Visualizations for data insights
•	Project report (this document)
