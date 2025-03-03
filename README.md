# <mark>**THIS REPO IS CURRENTLY UNDER CONSTRUCTION!** Check by after March 7th for updates to analysis and data visualizations. Thanks!</mark> 

# Amazon Transactions Dataset Analysis-Preliminary Draft

[![License](https://img.shields.io/badge/License-CC0-lightgray.svg?style=flat-square)](https://creativecommons.org/publicdomain/zero/1.0/) ![GitHub last commit](https://img.shields.io/github/last-commit/ambermocalis/Amazon_Transactions)

## Summary of Findings
This analysis explores purchasing behavior on Amazon, focusing on the correlation between demographics (age, income, education level) and product categories purchased. The findings suggest that demographic factors significantly influence purchase decisions, with certain age groups and income levels showing preferences for specific product types. Additionally, regional variations in product choices and spending behavior were identified. 

---

## Background of Data
The dataset consists of two main parts:
- **Amazon Transactions**: Data on products purchased, including product categories, price, and quantity.
- **Demographic Information**: Information on respondents' age, income, education, and location.

The two datasets can be linked through the "Survey ResponseID" field.

The data was voluntarily shared by individuals who reported their Amazon purchases, and it is intended for analysis of consumer behavior.

---
## Code
The analysis uses Python, with libraries such as `pandas`, `matplotlib`, and `seaborn` to process and visualize the data. You can find the full code in the `analysis.py` script.

---
## Large Dataset Storage
Due to GitHub's file size limits, the dataset is hosted externally.  
Download the dataset from [Harvard Dataverse](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/YGLYDY) before running the analysis.

---

## See Analysis with GitHub
### Option 1: Access GitHub.dev (Web-Based Editor)
GitHub.dev allows you to edit code directly in your browser without needing to install anything.
#### **1. Go to the GitHub Repository**  
   - Open your web browser and navigate to the GitHub repository you want to edit.  
#### **2. Open GitHub.dev**  
   - Press the `.` (period) key on your keyboard while viewing the repository.  
   - Alternatively, change the URL from github.com to github.dev (e.g., `https://github.com/user/repo` → `https://github.dev/user/repo`).
#### **3. Start Editing**  
   - GitHub.dev will launch a browser-based VS Code editor. 
   - Install the Malloy editor when prompted
   - You can now browse and edit files. Start with **IPEDS Data Analysis.malloynb**


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
- Begin working with this IPEDS data analysis notebook.
---

# Licensing
The code and analysis in this respository are distributed under the terms of the [Creative Commons 1.0 Universal license (CC0)](LICENSE).

# References
1. Alex Berke; Dan Calacci; Robert Mahari; Takahiro Yabe; Kent Larson; Sandy Pentland, 2023, "Open e-commerce 1.0: Five years of crowdsourced U.S. Amazon purchase histories with user demographics", Harvard Dataverse, V1, [Link](https://doi.org/10.7910/DVN/YGLYDY).