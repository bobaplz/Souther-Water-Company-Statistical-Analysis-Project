# Souther-Water-Company-Statistical-Analysis-Project
#Python # Exploratory Data Analysis #Descriptive Statistics #Regression model # Inferential Statistics#Pandas #Matplotlib #Seaborn #Statsmodels #Jupyternotebook #OLS Multivariate Regression Model #Prediction Validation

Metadata:
Data set: 'DF_Raw_Data.csv' and 'DF_Rolling_Stdev.csv'

Columns: 10(8 different Pump readings of Surjek with PUMP FAILURE (0 and 1) and TIMEFRAME (DD/MM/YYYY)).

Rows: 2453

This case study is divided into one financial analysis and two Statistical analyis.

Financial Analysis //

Ultimately, to tell a meaningful story that drives meaningful insights. 
For Southern Water Corp. I will measure my analytical su1ccess by ensuring you can tell Southern Water Corp. a meaningful story that unpacks
the EBIT, Revenues, and Operational Expenses at a macro and micro level.
This analysis is broken up into three (3) overall components. I have analyzed the subsequent revenues, operational expenses, EBIT, and tell the overall story the company has uncovered.


Statistical Anaysis //

1) Exploratory Data Analysis: Where we will perform Descriptive Statistical Analysis to identify the size,
    type, mean, median and quartiles which will help us to identify if any skewness (outliers) in the 
    dataframe. In this analysis we will be using  Seaborn boxplot to visualize the spread of dataframe and identify outliers. Since, we are tying to identify the predictive signals of pump failure, which meand the abnormalities in the readings, it is obvious that we will have outliers as indication of pump failure.
    Hence, in this case we will not remove the outliers from the dataset. Hovever to make our 
    Timeseries plotting more uniform we will be using Rolling Standard Deviation data set with an 
    interval of 30 seconds. 
    
2) Multivariate regression Model:In this data analysis, we will use OLS Regression Model in the 
    statsmodel.api library, to create a regression equation that models the Pump Failure (Y-Variable) against 
    all the independent variables, which include every other variable that is not PUMP FAILURE (1 or 0).
    We will be using Seaborn (heatmap) with (corr) function which will give us R- Squared values. 
    R-Squared colser to 1 = highest correlation w.r.t. pump failure. We will use the correlation coefficient 
    values of each pumps to calculate multivariate regression model by using OLS Regression Model to 
    predict pump failure patterns and validate that prediction by calculating coefficient matrix.
