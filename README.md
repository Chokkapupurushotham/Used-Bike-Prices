# Used-Bike-Prices

USED BIKE PRICES ANALYSIS USING FEATURE ENGINEERING AND EXPLORATORY DATA ANALYSIS

PROJECT OVERVIEW

This project focuses on analyzing the factors that influence the selling prices of used bikes in India. It uses real-world data collected from online listings and applies advanced data cleaning, feature engineering, and exploratory data analysis techniques to extract insights. The goal is to understand how attributes such as brand, mileage, power, and engine capacity affect resale prices, and to prepare the dataset for potential predictive modeling.
This project is positioned from the lens of a financial analyst using data science tools to support market evaluation, product valuation, and future pricing strategies.

OBJECTIVES

Clean and transform raw used bike listing data into a structured format

Explore patterns and trends in mileage, power, and price

Create meaningful features such as bike age and power-to-weight ratio

Handle missing and inconsistent entries for better data integrity

Analyze the influence of various features on bike price

Prepare the dataset for regression modeling


TOOLS AND TECHNOLOGIES USED

Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Regular Expressions)

Jupyter Notebook / Visual Studio Code

Domain Context: Finance and Pricing Analytics


DATA DESCRIPTION

The dataset contains listings for 7,857 used bikes and includes the following variables:

model_name: Complete bike model name including brand and year

model_year: Year of manufacturing

kms_driven: Total kilometers driven

owner: Owner type (first, second, etc.)

location: City or region where the bike is being sold

mileage: Mileage in kilometers per liter (kmpl)

power: Horsepower or brake horsepower (BHP)

cc: Engine displacement in cubic centimeters

price: Selling price in Indian Rupees

brand: Brand extracted from the model name


DATA CLEANING AND PREPARATION

Several critical data engineering steps were applied:

Missing values: Handled using domain knowledge or by imputing average values by brand

Inconsistent formats: Cleaned mileage, power, and kms_driven fields by removing units and converting to numeric types

Brand extraction: Extracted brand names from the model_name string

CC extraction: Parsed model names to infer engine capacity

Encoding categorical values: Used one-hot encoding for features like owner and location

Feature corrections: Standardized inconsistent naming formats and corrected power units


FEATURE ENGINEERING

New features were created or transformed:

bike_age: Calculated using the difference between the current year and model year

power-to-weight ratio: Suggested as a potential feature for advanced modeling

brand standardization: Ensured brand names are consistent

mileage and power standardization: Unified into numeric formats


EXPLORATORY DATA ANALYSIS

Year-wise Distribution
A bar plot showed that bike listings peaked around 2015. Newer models were listed less frequently.

Brand-wise Distribution
Bajaj and Royal Enfield were the most frequently listed brands.

Owner Type Analysis
Most bikes were sold by first owners, which usually implies better condition.

Engine Capacity Distribution (cc)
150cc and 350cc bikes were most common, with 1000cc+ models being rare.

STATISTICAL SUMMARY

Average mileage: 44.6 kmpl

Average power: 20.8 bhp

Average kms driven: 23,090 km

Average price: ₹1,06,791

Price range: ₹42,000 to ₹30+ lakhs


INSIGHTS AND OBSERVATIONS

Engine capacity has a strong influence on price

Brand and perceived reliability impact resale value

First-owner bikes have higher average prices

Power and mileage show moderate correlation with price


DATA READINESS FOR MODELING

No missing values

All features cleaned and converted

Dataset structured and suitable for regression models


NEXT STEPS AND RECOMMENDATIONS

Train regression models (Linear, Random Forest, XGBoost)

Evaluate using MSE, MAE, R-squared

Consider advanced tuning and deployment

Build dashboard for real-time valuation insights


CONCLUSION

This project transformed raw used bike listing data into a high-quality dataset through cleaning, feature engineering, and analysis. It reveals the key drivers of resale price and provides a strong foundation for building predictive models. These findings support better pricing strategies in the Indian two-wheeler market.
