# Retail Store Sales Analysis

## Project Overview

This project analyses retail store sales data using Python and Pandas.

The aim was to clean the dataset, investigate sales patterns and create visualisations to answer five analysis questions.

## Dataset

The original dataset contains 12,575 rows and 11 columns.

The columns are:

* Transaction ID
* Customer ID
* Category
* Item
* Price Per Unit
* Quantity
* Total Spent
* Payment Method
* Location
* Transaction Date
* Discount Applied

## Questions and Hypotheses

### Question 1

Which product category generates the highest total revenue?

**Hypothesis:** Electric household essentials generate the highest revenue.

### Question 2

Do online transactions generate more revenue than in-store transactions?

**Hypothesis:** Online transactions generate more revenue than in-store transactions.

### Question 3

Which payment method has the highest average transaction value?

**Hypothesis:** Credit-card transactions have the highest average transaction value.

### Question 4

Do customers spend more when a discount is applied?

**Hypothesis:** Discounted transactions have a higher average total spend.

### Question 5

How did monthly sales revenue change between 2022 and 2025?

**Hypothesis:** Monthly sales revenue increased over time.

## Data Exploration

Pandas was used to:

* Display the first rows of the dataset
* Check the number of rows and columns
* Check the data types
* Generate summary statistics
* Identify missing values
* Check for duplicate records

The dataset contained no duplicate rows.

Missing values were found in:

* Item
* Price Per Unit
* Quantity
* Total Spent
* Discount Applied

## Data Cleaning

The following cleaning steps were completed:

* A copy of the original DataFrame was created.
* Missing prices were calculated using total spending and quantity.
* Rows without quantity and total-spending values were removed.
* Missing item names were changed to `Unknown`.
* Missing discount values were changed to `Unknown`.
* Transaction dates were converted into datetime values.
* The cleaned dataset was saved as a new CSV file.

The cleaned dataset contains 11,971 rows and 11 columns.

## Visualisations and Findings

### 1. Revenue by Product Category

The Butchers category generated the highest total revenue at approximately £208,118.

This contradicted the hypothesis that electric household essentials would generate the highest revenue.

### 2. Revenue by Location

Online transactions generated approximately £791,401 in revenue. In-store transactions generated approximately £760,670.

This supported the hypothesis that online transactions generate more total revenue than in-store transactions.

### 3. Average Spending by Payment Method

Cash transactions had the highest average transaction value at approximately £131.05.

This contradicted the hypothesis that credit-card transactions would have the highest average value. However, there was only a small difference between the payment methods.

### 4. Spending by Discount Status

Discounted transactions had an average value of approximately £130.49. Transactions without a discount had an average value of approximately £129.95.

This slightly supported the hypothesis that discounts increase spending. However, the difference was very small.

### 5. Monthly Sales Over Time

Sales fluctuated rather than increasing continuously.

Total revenue was approximately:

* £510,330 in 2022
* £491,312 in 2023
* £524,881 in 2024

The 2025 data was incomplete because the dataset only contained transactions up to 18 January 2025.

The results did not clearly support the hypothesis that sales consistently increased over time.

## Technologies Used

* Python
* Pandas
* Matplotlib
* Seaborn
* Jupyter Notebook
* GitHub Codespaces

## Installation

Clone the repository:

```bash
git clone <git@github.com:ZAshter/git-example.git>
```

Install the required packages:

```bash
pip install pandas matplotlib seaborn
```

Open `project.ipynb` and run the notebook cells in order.

## Project Files

```text
retail_store_sales.csv
cleaned_retail_store_sales.csv
project.ipynb
README.md
```

## Conclusion

This project demonstrated how Python and Pandas can be used to clean, analyse and visualise retail sales data.

The analysis found that the Butchers category generated the highest revenue and online transactions generated slightly more revenue than in-store transactions. Payment method and discount status only had a small relationship with transaction value.

Monthly sales varied throughout the dataset, with the highest complete annual revenue recorded in 2024.
>>>>>>> 05e1d69 (finished the task)
