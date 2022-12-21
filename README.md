# Souther-Water-Company-Statistical-Analysis-Project
#Python # Exploratory Data Analysis #Descriptive Statistics #Regression model # Inferential Statistics#Pandas #Matplotlib #Seaborn #Statsmodels #Jupyternotebook #OLS Multivariate Regression Model #Prediction Validation

Metadata:
Data set: 'DF_Raw_Data.csv' and 'DF_Rolling_Stdev.csv'

Columns: 10(8 different Pump readings of Surjek with PUMP FAILURE (0 and 1) and TIMEFRAME (DD/MM/YYYY)).

Rows: 2453

This case study is divided into one financial analysis, one market economics analysis, and two Statistical analyis.

## Financial Analysis :

For Southern Water Corp. I will measure my analytical success by ensuring I can tell Southern Water Corp. a meaningful story that unpacks the EBIT, Revenues, and Operational Expenses at a macro and micro level.
This analysis is broken up into three (3) overall components. I have analyzed the subsequent revenues, operational expenses, EBIT, and tell the overall story the company has uncovered.

* Relevant Files

(a) Southern Water Company [Financial Analysis Objective Statement] - 
This file is an objective statement written by me to understand the company's goal and to drill down into smaller breakdowns what to find in this project.  Please read this objective statement as an outlook of this project for the financial analysis.

(b) Southern Water Corp Financial Project_EBIT - 
There three separated parts in this master excel file for the financial analysis : 
a) Revenue Analysis b) Expenses Analysis c) EBIT Analysis

(c) Presentation Southern Water Corp_Financial Analysis - 
This is an overall outlook of what I have found from this project. 
Based on Excel Master file, I have created KPI in each segmentation and projected the relationships between chemical expenditures and water production actual by units.

-------------------------------------------------------------------------------------------------------------------------------


## Economics Analysis :

For market economic analysis, I’ll be measuring analytical success by ensuring I can clearly tell the executives at Southern Water Corp a meaningful story that unpacks the elasticity analysis between soft and hard water products. This is to be followed by a cost-effectiveness evaluation for each desalination plant and whether  I can clearly identify the best periods to perform a major outage.

* Relevant Files

(a) Southern Water Company [Market Economics Analysis Objective Statement] - This file is an objective statement written by me to understand the company's goal and to drill down into smaller breakdowns what to find in this project. Please read this objective statement as an outlook of this project for the Market Economics Analysis.

(b) Southern Water Corp Market Economics Analysis - There three separated parts in this master excel file for the economics analysis : a) What-If Analysis b) Economics Market Analysis c) Economics Cost Analysis

(c) Presentation Southern Water Corp Economics - This is an overall outlook of what I have found from this project. Based on Excel Master file, I have created KPI in each segmentation and analyzed the elasticity patterns in between Hard Water and Soft Water products.


-------------------------------------------------------------------------------------------------------------------------------


## Statistical Anaysis :

1 -- Exploratory Data Analysis

Where I will be performing Descriptive Statistical Analysis to identify the size, type, mean, median and quartiles which will help us to identify if any skewness (outliers) in the dataframe. In this analysis I will be using Seaborn boxplot to visualize the spread of dataframe and identify outliers. Since, I am trying to identify the predictive signals of pump failure, which meand the abnormalities in the readings, it is obvious that we will have outliers as indication of pump failure.
Hence, in this case I will not remove the outliers from the dataset. However, to make the Timeseries plotting more uniform I will be using Rolling Standard Deviation data set with an interval of 30 seconds. 

2 -- Multivariate regression Model

In this data analysis, I will use OLS Regression Model in the statsmodel.api library, to create a regression equation that models the Pump Failure (Y-Variable) against 
all the independent variables, which include every other variable that is not PUMP FAILURE (1 or 0). I will be using Seaborn (heatmap) with (corr) function which will give us R- Squared values. R-Squared closer to 1 = highest correlation w.r.t. pump failure. I will use the correlation coefficient values of each pumps to calculate multivariate regression model by using OLS Regression Model to predict pump failure patterns and validate that prediction by calculating coefficient matrix.

* Relevant Files

(a) Southern Water Company [Statistics Analysis Objective Statement] - This file is an objective statement written by me to understand the company's goal and to drill down into smaller breakdowns what to find in this project. Please read this objective statement as an outlook of this project for the Statistics Analysis.

(b) Southern Water Corp Statistics Analysis - There two separated parts in this master excel file for the statistics analysis : a) Descriptive Statistics b) Inferential Statistics 

(c) Presentation Southern Water Corp Statistics - This is an overall outlook of what I have found from this project. Based on Excel Master file, I have detected the correlations among the operational factors which make negative impact on water pump failure.

## (d) Southern Water Corp OLS Statistics Analysis in Python 
- I revisited the Pump Data from Statistics Analysis above and added more sophisticated work with Python in order to automate the process for the future use.
- Used Jupyter Notebook
- Included both descriptive statistics and inferential statistics
- Included box plot, correlation heatmap, bar/line plot, timeframe chart
