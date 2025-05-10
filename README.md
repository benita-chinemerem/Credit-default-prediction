# Credit Default Prediction Project

This is my final project for the **Introduction to Machine Learning** course.  
The project aims to predict whether a customer will default on their credit card or loan using financial data from Amex.

---

## What is This Project About?

In simple terms, banks and lenders want to know:  
*"If I lend money to this person, will they pay me back?"*  

This project uses different machine learning models to analyze customer financial data and predict whether they're likely to default (not pay back) their debt.

---

## Challenges Encountered

1. **Dataset Size**:  
   Instead of working with the full 5.5 million-row dataset, I sampled it down to 40,000 customer records to make the analysis manageable.

2. **Anonymized Data**:  
   All the data is anonymized. Instead of seeing features like "income" or "age," the dataset contains cryptic codes like "D_87" or "P_2."  
   This made the analysis feel like solving a puzzle without knowing what the pieces represent!

---

## Feature Characteristics and Data Description

The dataset includes 190 different pieces of information about each customer, grouped into 5 categories:

- **Delinquency (D)**: How often they've missed payments (87 features)  
- **Spending (S)**: Their spending habits (21 features)  
- **Payment (P)**: How they pay their bills (3 features)  
- **Balance (B)**: Their account balances (40 features)  
- **Risk (R)**: Other risk indicators (28 features)  

---

## What I Discovered From the Data Analysis

1. **Missing Information is Actually Information**:  
   Some data fields were almost completely empty (missing 99.9% of the time).  
   Instead of ignoring these, I realized that missing data might actually tell us something important about a customer.

2. **Some Features Work Together**:  
   Certain features are highly correlated. For example, if one feature shows a customer misses payments often, other features show similar patterns.  
   This helped simplify the analysis.

3. **One Feature Stands Out**:  
   Feature **"P_2"** turned out to be especially good at predicting defaults.  
   It had a **-61% correlation** with default, meaning when this number is high, customers are much less likely to default.

---

## My Approach

I used Jupyter notebooks to:

1. Explore the data and understand patterns.  
2. Clean and prepare the data for analysis.  
3. Build and test different prediction models.  
4. Compare our results with other successful approaches.

---

## Learning From Others

We looked at what worked for other Kagglers in this competition:

- Some kept all 190 features and achieved **89.67% accuracy**.  
- Others reduced features to 89 and still achieved **89.6% accuracy**.  
- The best approach used 168 features and achieved **93.42% accuracy**.  

This taught me that success isn't just about having more data—it's about finding the right balance.

---

## Results Summary

1. Identified key patterns in customer behavior.  
2. Found that missing data can be meaningful.  
3. Discovered which features are most important for prediction.  
4. Successfully reduced complexity while maintaining accuracy.

---

## How to Use This Project

1. Open the Jupyter notebooks to see the analysis.  
2. Run the code cells to reproduce the findings.  
3. Check out the presentation for a high-level summary.

---

## Why This Matters

Better credit default prediction means:

- Banks can lend money more safely.  
- Deserving customers get approved for loans.  
- Interest rates can be set more fairly.  
- Everyone benefits from more accurate risk assessment.