Credit Default Prediction Project
This is my final project for Introduction to machine learning course.
This project aims to helps predict whether a customer will default on their credit card or loan using financial data from Amex.
What is this project about?
In simple terms, banks and lenders want to know: "If I lend money to this person, will they pay me back?"
This project uses different machine learning models to look at customer financial data and predict whether they're likely to default (not pay back) their debt.

*Challenge that I encountered:
Instead of working with the 5.5 million row dataset, I sampled it down to 40,000 customer records to make my analysis manageable. Also what is tricky about this data is that All the data is anonymized - meaning instead of seeing "income" or "age", I would see cryptic codes like "D_87" or "P_2". It's more like trying to solve a puzzle without knowing what the pieces represent!

Feature characteristics and data description?
The data includes 190 different pieces of information about each customer, grouped into 5 categories:

Delinquency (D): How often they've missed payments (87 features)
Spending (S): Their spending habits (21 features)
Payment (P): How they pay their bills (3 features)
Balance (B): Their account balances (40 features)
Risk (R): Other risk indicators (28 features)

##What I discovered from analysis of the data##:
1. Missing Information is Actually Information!
Some data fields were almost completely empty (missing 99.9% of the time). Instead of ignoring these, I realized that having no data might actually tell us something important about a customer.
2. Some Features Work Together
We found that certain features are very similar to each other. For example, if one feature shows a customer misses payments often, there are other features that show the same pattern. This helped us simplify our analysis.
3. One Feature Stands Out
Feature "P_2" turned out to be especially good at predicting defaults. It had a -61% correlation with default, meaning when this number is high, customers are much less likely to default.

##My Approach##
I used Jupyter notebooks to:

Explore the data and understand patterns
Clean and prepare the data for analysis
Build and test different prediction models
Compare our results with other successful approaches

##Learning from Others##
We looked at what worked for other kagglers for this competition:

Some kept all 190 features and got 89.67% accuracy
Others reduced features to 89 and still got 89.6% accuracy
The best approach used 168 features and achieved 93.42% accuracy

This taught me that success isn't just about having more data - it's about finding the right balance.

##Results Summary##

Identified key patterns in customer behavior
Found that missing data can be meaningful
Discovered which features are most important for prediction
Successfully reduced complexity while maintaining accuracy

##How to Use This Project##

Open the Jupyter notebooks to see our analysis
Run the code cells to reproduce our findings
Check out our presentation for a high-level summary

##Why This Matters##
Better credit default prediction means:

Banks can lend money more safely
Deserving customers get approved for loans
Interest rates can be set more fairly
Everyone benefits from more accurate risk assessment