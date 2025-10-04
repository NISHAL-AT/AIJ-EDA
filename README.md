Salary Outlier Detection using AI

![Python](https://img.shields.io/badge/Python-3.11-blue)
![Pandas](https://img.shields.io/badge/Pandas-1.5.3-green)
![NumPy](https://img.shields.io/badge/NumPy-1.26.0-orange)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.3.2-yelllow)

Table of Contents
- [Project Description](#project-description)
- [Dataset](#dataset)
- [Screenshots / Results](#screenshots--results)
- [Features](#features)
- [How It Works](#how-it-works)
- [Installation](#installation)
- [Usage](#usage)
- [Technologies Used](#technologies-used)
- [Author](#author)

Project Description
This project detects salary outliers in a dataset using statistical and machine learning methods. It highlights anomalies to help organizations analyze salary distribution and make informed decisions. The project also handles missing data and provides visual insights.

Dataset
- Dataset contains salary information in USD.
- Missing values and outliers are automatically handled and highlighted.
- Columns include `Salary_USD`, `Department`, `Location`, etc.

Screenshots / Results
Here are some screenshots from the project:

![Salary Outlier Plot](images/industry_count.png)  
*Visual representation of industry count in the dataset.*

![Data Overview](images/salary_boxplot.png)  
*Summary of dataset showing salary distirbutions.*

Features
- Detects outliers automatically using IQR or z-score methods
- Handles missing data efficiently
- Provides visualizations for better understanding
- Scalable for large datasets

How It Works
1. Load the dataset using Pandas.
2. Handle missing values and create indicator columns for missing data.
3. Detect outliers using IQR or z-score

Installation:

Clone the repository:
    git clone <your-repo-link>
Navigate to the project folder:
    cd project-folder
Install dependencies:
    pip install -r requirements.txt

Technologies Used:
     Python
     Pandas
     NumPy
     Matplotlib / Seaborn
     Scikit-learn
   
   df['Salary_USD_outlier'] = ((df['Salary_USD'] < lower_bound) | (df['Salary_USD'] > upper_bound)).astype(int)
