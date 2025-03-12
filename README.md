# Customer-Purchase-Data-Analysis
## Ecommerce Purchases Exercise
## Overview

This assignment involves analyzing a dataset of customer purchase information from an e-commerce platform. The dataset contains 30,000 entries with 20 columns, including customer details (name, email, gender, age, etc.), purchase information (price, credit card details, etc.), and additional metadata (IP address, favorite color, etc.). The goal is to answer specific questions about the dataset using Pandas, a powerful data manipulation library in Python.

## Files
- `Cust_Purch_FakeData.csv`: The raw customer purchase data file.
- `Cust_Purch_Data_Assign.ipynb`: Data analysis file.

## Methodology
1. Data Loading: The dataset is loaded into a Pandas DataFrame using pd.read_csv().
2. Data Exploration: Basic exploration is performed using methods like .head(), .shape, and .info() to understand the structure of the dataset (e.g., number of rows, columns, and data types).
3. Data Analysis: Filtering rows based on conditions (e.g., cust[cust['phone'] == '(263) 382-8004']). Using .value_counts() to find the frequency of unique values (e.g., most common customer names or professions). Calculating summary statistics (e.g., max, min, and average spending using .max(), .min(), and .mean()).
4. Advanced Filtering: Lambda functions are used for advanced filtering (e.g., extracting email domains using apply(lambda x: x.split('@')[1])).

## Findings
- `Dataset Overview`: The dataset contains 30,000 entries and 20 columns. Columns include customer details (e.g., name, email, gender, age), purchase information (e.g., price, credit card details), and metadata (e.g., IP address, favorite color).
- `Customer Demographics`: The maximum age of customers is 65, the minimum age is 18, and the average age is 41.55. The three most common customer names are Willie, Francis, and Eula.
- `Shared Phone Number`: Two customers share the same phone number: (263) 382-8004. These customers are:
**Lilly Tyler (Female, 38 years old, Structural Engineer) &**
**Peter Cain (Male, 27 years old, Insurance Adjuster)**
- `Professions`: The two most common professions are Preschool Teacher (112 occurrences) and Distribution Manager (107 occurrences). There are 87 customers with the profession Structural Engineer, out of which 43 are male.
- `Spending Analysis`: The maximum spending is 100 CAD, the minimum spending is 0 CAD, and the average spending is 49.99 CAD. Two customers did not spend anything:
**Bruce Bryan (Male, 59 years old, Engineer Technician) &**
**Flora Clark (Female, 27 years old, Cruise Director)**
- `Credit Card Information`: 1,721 customers use Visa as their credit card provider. One customer spent 100 CAD using a Visa card: Gregory Brown (Female, 31 years old, Novelist)
- `Email Analysis`: The top 5 most popular email providers are:
1. gmail.com (1,687 customers), 
2. me.com (1,676 customers), 
3. outlook.com (1,664 customers), 
4. live.com (1,660 customers) &
5. hotmail.com (1,659 customers).
One customer uses an email with the domain am.edu:
Loretta Fletcher (Female, 48 years old, Rehabilitation Counselor)
- `Store Traffic`: The store receives the most customers on Saturday (4,376 customers), followed by Wednesday (4,365 customers).

So finally, these insights can help the e-commerce company make data-driven decisions, such as targeting specific customer segments or improving marketing strategies.
