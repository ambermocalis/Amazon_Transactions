# <mark>**THIS REPO IS CURRENTLY UNDER CONSTRUCTION!** Check by after March 7th for updates to analysis and data visualizations. Thanks!</mark> 

# Amazon Transactions Dataset Analysis-Preliminary Draft

## 1. Summary of Findings
This analysis explores purchasing behavior on Amazon, focusing on the correlation between demographics (age, income, education level) and product categories purchased. The findings suggest that demographic factors significantly influence purchase decisions, with certain age groups and income levels showing preferences for specific product types. Additionally, regional variations in product choices and spending behavior were identified. 

## 2. Background of Data
The dataset consists of two main parts:
- **Amazon Transactions**: Data on products purchased, including product categories, price, and quantity.
- **Demographic Information**: Information on respondents' age, income, education, and location.

The two datasets can be linked through the "Survey ResponseID" field.

The data was voluntarily shared by individuals who reported their Amazon purchases, and it is intended for analysis of consumer behavior.

## 3. Code
The analysis uses Python, with libraries such as `pandas`, `matplotlib`, and `seaborn` to process and visualize the data. You can find the full code in the `analysis.py` script.

### Example Code Snippet:
```python
import pandas as pd
import matplotlib.pyplot as plt

# Load datasets
transactions = pd.read_csv('transactions.csv')
demographics = pd.read_csv('demographics.csv')

# Merge datasets on 'Survey ResponseID'
merged_data = pd.merge(transactions, demographics, on='Survey ResponseID')

# Analyze and visualize spending based on age
age_spending = merged_data.groupby('Age')['Total Spent'].sum()
age_spending.plot(kind='bar')
plt.title('Total Spending by Age Group')
plt.xlabel('Age Group')
plt.ylabel('Total Spending')
plt.show()
