## Project Description

This project is an AOL (Assurance of Learning) course Introduction to data science. Assignment aimed at understanding demographic representation trends from the 1994 United States Census Data. The primary goal of this analysis is to build a predictive model capable of classifying whether an individual earns more or less than USD 50,000 per year. Through this project, we hope to gain deeper intuition behind these demographic figures

## Dataset Information

The dataset used comes from the 1994 United States Census Database from UCI Machine Learning Repositories. This Dataset originally contained approximately 48,842 data entries. The target feature in this project is the "income_>50K" column, which contains the income classification of the census participants

## Data Processing (Data Cleaning) Steps

The raw data used was previously modified to contain missing values, inconsistent data, and duplicates. The following data cleaning stages were performed:

* Importing core libraries such as Pandas, NumPy, SciPy, Matplotlib, and Seaborn.
* Removing duplicated data rows using the drop_duplicates() function.
* Identifying and removing missing values (NaN) in variables like native-country, capital-gain, capital-loss, occupation, and workclass using the dropna() function.
* Dropping variables/columns deemed unnecessary for visualization, including: native-country, fnlwgt, educational-num, and race.
* Standardizing inconsistent data in the gender column (converting 'M' and 'Man' to 'Male', and 'F' and 'Woman' to 'Female').
* Standardizing inconsistent data in the workclass column (converting 'State-gov_' to 'State-gov', and '/Private' to 'Private').
* Transforming the binary values of the classification target income_>50K into categorical format ('No' for 0, and 'Yes' for 1).
* Detecting and removing outliers in the capital-gain and capital-loss columns using the Interquartile Range (IQR) method.

## Data Analysis & Visualization

Once the data was cleaned, the next stage involved visualizing it to interpret the findings. Some of the visualizations performed include:

* Boxplots to observe outlier distributions before and after applying the IQR method.
* A Pie Chart showing income distribution, revealing that 24.8% of the population has an income >50K and 75.2% has an income <=50K.
* A Histogram (KDE) to analyze the age distribution of the census participants.

## Technologies Used

* Programming Language: Python
* Data Manipulation: Pandas, NumPy
* Statistical Analysis: SciPy
* Data Visualization: Matplotlib, Seaborn
* Design: Canva

## Team Members

This Project was completed by Group 5:
1. Angela Kei Budiwinoto
2. Leora Natania Klarise Purba
3. Zahra Annisa Afandi
