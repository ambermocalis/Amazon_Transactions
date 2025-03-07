# Amazon Transactions Dataset Analysis

[![License](https://img.shields.io/badge/License-CC0-lightgray.svg?style=flat-square)](https://creativecommons.org/publicdomain/zero/1.0/) ![GitHub last commit](https://img.shields.io/github/last-commit/ambermocalis/Amazon_Transactions)

## About the Data & Analysis
This analysis explores the purchasing behavior of over 5,000 U.S. Amazon customers. The data was obtained through the use of an experimental survey seeking to crowdsource an open source dataset of customer demographics and purching behavior. The focus of that survey was to crowdsource the first ever opensource Amazon purchase and demographics dataset while, at the same time, testing various data collection methods for user acceptance in order to enhance future crowdsourcing efforts for academic research (Berke et al., 2024, para. 1). The purpose of this analysis is much simpler and focuses on the correlation between demographics (age, gender, race, income, education level, and geographic location) and product categories purchased on Amazon. 

### Summary of Findings
When it comes to purchasing products on Amazon, consumers think fast, inexpensive, and trustworthy. Not surprisingly, the dataset revealed that the average cost per unit for products purchased was $22.66. In fact, Amazon prices fall within an F-distribution of pricing, with most prices falling within the $1.50 to $35 range.
<p align="center">
<img alt="Price per unit distribution." width="50%" src="https://github.com/ambermocalis/Amazon_Transactions/blob/main/images/F-distribution_of_per_unit_price.png"><br>
<em>Figure: Screenshot of price per unit distribution.</em></p>

When it comes to what kinds of products customers are purchasing from Amazon, books sales take the top spot, selling over 125% more than the next leading sales category--pet food. Amazon enthusiasts may recall that Amazon actually started out as a book seller...so this analysis makes sense!
<p align="center">
    <img alt="Top 10 Sales Categories." width="45%" src="https://github.com/ambermocalis/Amazon_Transactions/blob/main/images/top_sales_categories.png">
    <img alt="Spark Chart of Sales Categories" width="45%" src="https://github.com/ambermocalis/Amazon_Transactions/blob/main/images/top_categories_spark.png">
</p>
<p align="center">
    <em>Figure: Two visuals of Amazon's Top 10 Sales Categories.</em>
</p>

The findings suggest that age and income demographic factors significantly influence purchase rates in terms of items purchased and total sales. 25-34 and 35-44 year olds account for more than 50% of item purchases each year and women outpace men in terms of volume and total cost of items purchased <mark>(see the malloynb file at the end of the "Age Group Purchasing Trends" section for a bonus insight on how 25-34, 35-44, and 45-54 year groups compare).</mark> 
<p align="center">
    <img alt="Purchases by Age Group." width="45%" src="https://github.com/ambermocalis/Amazon_Transactions/blob/main/images/purchases_by_age_group.png">
    <img alt="Purchase Categories by Age Group" width="45%" src="https://github.com/ambermocalis/Amazon_Transactions/blob/main/images/purchases_by_age_group_categories.png">
</p>
<p align="center">
    <img alt="Purchases by Gender" width="45%" src="https://github.com/ambermocalis/Amazon_Transactions/blob/main/images/purchases_by_gender.png">
    <img alt="Purchases by Education Level." width="45%" src="https://github.com/ambermocalis/Amazon_Transactions/blob/main/images/purchases_by_education.png">
</p>
<p align="center">
    <em>Figure: Screenshots of visualizations of Age, Gender, and Education Level.</em>
</p>

I found two things that seemed exceptional in the course of my analysis. The first, which was interesting, but not particularly surprising, was that median-income households made up the majority of consumer purchases on Amazon. I don't find it surprising that lower-income households (less than $25,000 annual income) purchase less on Amazon, since their purchasing power is more limited due to their reduced capacity for discretionary spending. Additionally, while correlation does not equal causation, higher income households (greater than $150,000 annual income) were shown to spend less on Amazon, possibly because they have enough discretionary income to source more expensive products in-store or through other retail services. This is speculation, and we would need additional data to confirm my hypothesis.
<p align="center">
<img alt="Purchasing Rates by Income Group." width="50%" src="https://github.com/ambermocalis/Amazon_Transactions/blob/main/images/purchases_by_income.png"><br>
<em>Figure: Screenshot of Income Levels and Purchasing Rates</em></p>

The second insight the data provided was absolutely fascinating to me: while the majority of respondents in this dataset were buying books, pet food, clothing and electronic accessories, the Native Hawaiian or Other Pacific Islander demographic was predominantly buying their foodstuffs through Amazon! Food, Water, Poultry, Fruit Snacks, and Snack Crisps/Chips were their top 5 categories. With the exception of Food, those categories don't even show up in the top 10 categories across the dataset population!
<p align="center">
    <img alt="Purchasing by Race-Spark Charts." width="45%" src="https://github.com/ambermocalis/Amazon_Transactions/blob/main/images/purchases_by_race_spark.png">
    <img alt="Purchases by Race-Category Snapshot" width="45%" src="https://github.com/ambermocalis/Amazon_Transactions/blob/main/images/purchases_variation_example.png">
</p>
<p align="center">
<img alt="Patterns in Geography and Purchasing by Race." width="90%" src="https://github.com/ambermocalis/Amazon_Transactions/blob/main/images/shape_map_race_patterns.png"><br>
</p>
<p align="center">
    <em>Figure: Surprising Insights Into Preferred Categories by Race.</em>
</p>

Finally, there is also a direct correllation between purchasing rate spikes and distinct Amazon sale periods, like Prime Deal Days and Black Friday or Cyber Monday sales. I spent minimal time exploring this trend. This could be an opportunity to expand on what I've started.
<p align="center">
    <img alt="Prime Deals Day Sales-2021." width="45%" src="https://github.com/ambermocalis/Amazon_Transactions/blob/main/images/prime_day.png">
    <img alt="Black Friday/Cyber Monday Sales-2021" width="45%" src="https://github.com/ambermocalis/Amazon_Transactions/blob/main/images/black_friday_cyber_monday.png">
</p>
<p align="center">
    <em>Figure: Two charts with a Malloy tooltip showing examples of sales spikes around key sale days.</em>
</p>

### Conclusion
This analysis just scratches the surface of potential in this dataset, but there is still some interesting information, especially regarding the correlation between income and purchasing as well as varying trends in the types of products customers buy based on their race. Future analysis on population percentages and mean income may produce further insights and is an opportunity for others to expand on this work.

#### Are you a fellow data nerd? Keep reading...
If you have suggestions of more analysis, please feel free to comment. You can also clone this repository and make your own contributions by starting a pull request. Or download the zip file to your own terminal and create your own analysis from where I've left off. Thank you so much for your interest in reading this analysis!
 

---

## Background of Data
The dataset consists of two main parts:
- **Amazon Transactions**: Data on products purchased, including product categories, price, and quantity.
- **Demographic Information**: Information on respondents' age, income, education, and location.

The two datasets are linked through the "Survey ResponseID" field.

The data was voluntarily shared by individuals who reported their Amazon purchases, and it is intended for analysis of consumer behavior.

---
## Code
You'll find two Malloy notebook files in the repo:
- **[AmazonTransactions_source.malloy](AmazonTransactions_source.malloy)** used to source all of the data tables for a clean import to analysis notebook.
- **[Amazon_Transactions.malloynb](Amazon_Transactions.malloynb)** is where you will find all of the code for analysis. 
---
## Large Dataset Storage
Due to GitHub's file size limits, the dataset is hosted externally.  
Download the dataset from [Harvard Dataverse](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/YGLYDY) before running the analysis.

---

## See Analysis with GitHub
### Option 1: Access GitHub.dev (Web-Based Editor)
###### **You may run into errors with this method due to .csv file sizes. I have tried to remedy these "fetch" errors, but if you run into more errors you can download the repo to your terminal**
GitHub.dev allows you to edit code directly in your browser without needing to install anything.
#### **1. Go to the GitHub Repository**  
   - Open your web browser and navigate to the GitHub repository you want to edit.  
#### **2. Open GitHub.dev**  
   - Press the `.` (period) key on your keyboard while viewing the repository.  
   - Alternatively, change the URL from github.com to github.dev (e.g., `https://github.com/user/repo` → `https://github.dev/user/repo`).
#### **3. Start Editing**  
   - GitHub.dev will launch a browser-based VS Code editor. 
   - Install the Malloy editor when prompted
   - You can now browse and edit files. Start with **Amazon_Transactions.malloynb**


### Option 2: Clone a GitHub Repository Using GitHub Desktop & Your Code Editor
If you prefer a local development environment, follow these steps:

#### **1. Install GitHub Desktop** (if you haven't already)
- Download and install **GitHub Desktop** from [desktop.github.com](https://desktop.github.com/).
#### **2. Clone the Repository**
- Open **GitHub Desktop**.
- Click **File** → **Clone Repository**.
- Choose **GitHub.com** and sign in if prompted.
- Select the repository you want to clone from the list.
- Choose a local directory for storing the repo.
- Click **Clone**.
#### **3. Open the Repository in Your Preferred Code Editor**
After cloning, you can open the repository in your favorite code editor:
- **In GitHub Desktop:**  
  - Click **Repository** → **Open in Your Editor** (e.g., VS Code, PyCharm, Jupyter Notebook).  
  - If the option isn’t available, manually open your editor and select the cloned folder.
- **Manually (for Any Editor):**  
  - Open your code editor.  
  - Navigate to **File** → **Open Folder** and select the cloned repository directory.  
#### **4. Start Your Analysis**
- Install the Malloy extension (if you haven't already).
- Begin working with the **Amazon_Transactions.malloynb** notebook.
---


# References
1. Amazon Staff. (2024, June 25). The history of Prime Day: A look back at Amazon’s biggest deal event of the summer. About Amazon. https://www.aboutamazon.com/news/retail/the-history-of-prime-day
2. Berke, A., Calacci, D., Mahari, R. Yabe, T., Larson, K., & Pentland, S. Open e-commerce 1.0, five years of crowdsourced U.S. Amazon purchase histories with user demographics. Sci Data 11, 491 (2024). https://doi.org/10.1038/s41597-024-03329-6
3. Berke, A., Mahari, R., Pentland, S., Larson, K., & Calacci, D. (2024). Insights from an experiment crowdsourcing data from thousands of US Amazon users: The importance of transparency, money, and data use. Proceedings of the ACM on Human-Computer Interaction, 8(CSCW2), 1–48. https://doi.org/10.1145/3687005

