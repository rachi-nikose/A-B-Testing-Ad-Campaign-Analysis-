# A/B Testing & Ad Campaign Performance Analysis: Facebook vs. AdWords
## Project Overview
This project analyzes the performance of Facebook and AdWords advertising campaigns through A/B testing to determine which platform yields better results in terms of clicks, conversions, and overall cost-effectiveness. The primary objective is to identify the more effective platform to help marketing agencies allocate resources efficiently and optimize advertising strategies for maximizing client Return on Investment (ROI).

Using Python and key data science libraries (Pandas, Scikit-learn, SciPy, Matplotlib, Seaborn, Statsmodels), this analysis identifies Facebook as the superior platform, nearly doubling average daily conversions (11.74 for Facebook vs. 5.98 for AdWords). The project also includes the development of a predictive model (76.35% R2 score) for Facebook conversions based on clicks and provides insights into cost-effective campaign timing.

## Key Findings & Highlights
Platform Performance: Facebook significantly outperformed AdWords in driving conversions, with an average of 11.74 daily conversions compared to AdWords' 5.98.

Predictive Modeling: A Linear Regression model was developed for Facebook ads, achieving an R2 score of 76.35% in predicting conversions from clicks (e.g., approximately 13 conversions can be expected from 50 clicks).

Engagement Correlation: Facebook demonstrated a strong positive correlation (0.87) between ad clicks and conversions, indicating higher engagement effectiveness than AdWords (0.45 correlation).

Cost-Effectiveness: Analysis of Cost Per Conversion (CPC) on Facebook identified May and November as the most cost-effective months for advertising.

High-Conversion Days: Facebook campaigns resulted in significantly more high-conversion days (e.g., 189 days with 10-15 conversions) compared to AdWords (0 days in the same bracket) over the 365-day analysis period.

Statistical Significance: Hypothesis testing (t-test) confirmed that the higher number of conversions from Facebook was statistically significant (p < 0.05).

Long-Term Relationship: Cointegration testing indicated a stable, long-term equilibrium relationship between advertising spend and conversions on Facebook.

## Tech Stack & Libraries Used
Python 3

Pandas: For data manipulation, cleaning, and analysis.

NumPy: For numerical operations.

Matplotlib & Seaborn: For data visualization (histograms, scatter plots, line charts, bar charts).

Scikit-learn (sklearn): For building the Linear Regression model and evaluating its performance (R2 score, MSE).

SciPy (scipy.stats): For performing hypothesis testing (independent samples t-test).

Statsmodels: For time series analysis, specifically cointegration testing.

Jupyter Notebook: For interactive data analysis and presentation.

## Project Workflow
Business Problem Definition: Determine which ad platform (Facebook vs. AdWords) is more effective.

Data Extraction & Loading: The marketing_campaign.csv dataset was loaded into a Pandas DataFrame.

Data Cleaning & Preprocessing:

Converted 'Date' column to datetime objects.

Cleaned numerical columns by removing currency/percentage symbols and converting to float types.

Performed initial data exploration (.head(), .shape, .dtypes, .describe()).

Exploratory Data Analysis (EDA):

Visualized distributions of clicks and conversions.

Created conversion categories for frequency analysis.

Analyzed correlations between clicks and conversions.

Examined weekly and monthly trends for conversions and CPC.

Statistical Analysis & Modeling:

Hypothesis Testing: Compared mean conversions between Facebook and AdWords.

Regression Analysis: Predicted Facebook ad conversions from clicks.

Time Series Analysis: Assessed the long-term relationship between ad spend and conversions on Facebook.

Interpretation & Conclusion: Drew insights from the analysis to answer the research question and provide actionable recommendations.

### Dataset
The analysis is based on the marketing_campaign.csv file, which contains daily performance data for both Facebook and AdWords ad campaigns throughout the year 2019 (365 days). Key features include:

Date

Ad Views

Ad Clicks

Ad Conversions

Cost per Ad

Click-Through Rate (CTR)

Conversion Rate

Cost per Click (CPC)

### How to Use
Clone this repository.

Ensure you have Python and the necessary libraries (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, SciPy, Statsmodels) installed.

Open and run the AB Testing (Marketing Campaigns).ipynb Jupyter Notebook to see the full analysis, code, and visualizations.

The marketing_campaign.csv file should be in the same directory as the notebook or the path should be updated accordingly.

### Conclusion & Recommendations
The analysis conclusively demonstrates that the Facebook advertising campaign was more effective in terms of conversions and exhibited a stronger relationship between clicks and sales compared to the AdWords campaign during the analyzed period. 
Businesses are recommended to consider reallocating advertising resources towards Facebook and optimizing campaigns during identified cost-effective months (May and November) to maximize ROI. The predictive model for Facebook can further aid in setting realistic campaign goals.
