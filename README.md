# Housing-Data-analysis

## Overview
Applied feature engineering techniques to find the factors that influence price negotiations
while buying a house. 
Seggergated the source data in to numerical(continuous) and categorical(discrete) dataframes and used pearson correlation method to find out the correlation amongst the numerical data. Used OneHot Encoding to prepare the categorical dataframe for further testing and determined the P-Value to perform the Chi square test on the categorical fields to finally realise what are the important variable fields

#### Methods involved 
1. Pearson Correlation principle
2. OneHot Encoding
3. Chi-Square test (P-Value)
4. Data Viz using Pairplot, Boxplot, Countplot and Heatmap

## Dataset overview
There are a total of 80 variable fields in the dataset, some of which are listed below - 
1. MsZoning : Identifies the general zoning classification of the sale | 
2. MsSubclass : Identifies the type of dwelling involved in sale | 
3. LotFrontage : Linear feet of street connected to property | 
4. LotArea : Lot size in square feet | 
5. Street : Type of road access to property | 
6. Alley : Type of alley access to property | 
7. Neighborhood : Physical locations within the city limits | 
8. Foundation : Type of foundation | 
9. ExterCond : Evaluates the present condition of the material on the exterior | 
10. BsmntQual : Evaluates the height of the basement

## Findings
1. GarageCars and GarageArea are highly correlated with each other hence we'll drop one feature from these two which has less correlation value with the sale price. 
2. TotalBsmtSF and 1stFlrSF are also highy correlated with each other hence we'll drop one feature from these two which has less correlation value with the sale price. 
3. TotRmsAbvGrd and GrLivArea are also highly correlated with each other hence we'll drop one feature from these two which has less correlation value with the sale price. 
4. Also We can drop both FullBath and YearRemodAdd features as well as these feautures inter-correlated with other features.

## Conclusion
A total of 24 columns out of the initial 80 variable fields have been dropped since they are not in any case useful for any type of analysis as they do not correlate or impact our target field, sale price. In the end after cleaning and analysing our dataset we are finally left with 56 variable fields that can be important to us and maybe loaded in to our database for further investigation.
