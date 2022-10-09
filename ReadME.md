# Project 2: Predicting Housing Prices with Linear Regression

#### _Rohazeanti Mohamad Jenpire_

### Problem Statement
Real estate agents or brokers utilize Comparative Market Analysis, [*CMA*](https://www.investopedia.com/terms/c/comparative-market-analysis.asp), to present clients with a proposed sale price and a comprehensive justification for the price. It is an estimate of a home's value based on recently sold, similar properties in the immediate area. 


Even with such analytics tool available, many brokers applied personal experience and intuition when presenting proposed price to home buyers. Our analysis aims to create a regression model for pricing homes closer to their "real value" in the Ames, Iowa housing market. There are various websites that such as [*Zillow.com*](https://www.zillow.com/) and [*Trulia.com*](https://www.trulia.com/) that provide estimates on the market value of a particular property.

Our analysis will build a model specifically for Ames, Iowa, that real estate brokers can utilize on top of CMA reports to me more confident in their proposed price with an objective of predicting the price of housing in Ames,  with higher accuracy and more features.

### Executive Summary
This project explores Ames Dataset which contains contains information from the Ames Assessor’s Office used in computing assessed values for individual residential properties sold in Ames, IA from 2006 to 2010. The data has 82 columns which include 23 nominal, 23 ordinal, 14 discrete, and 20 continuous variables 

Exploratory data analysis revealed a seemingly strong positive correlation between the Sale Price and Overall Quality and size of Ground Living Area amongst many others. Exploratory data analysis also revealed that there is a strong negative correlation between Sale Price and age of the house which is expected. Older houses tend to be have lower overall quality and condition which affects price. 

Our data model is able to predict price of house with features such as location in a neighborhood, overall quality of the house, presence of fireplace and its quality as and even based on the when the house was last remodeled. 

### Data Sources
For this project, these are the datasets used:

[train](./datasets/train.csv)

[test](./datasets/test.csv)

### Data Dictionary
Data dictionary can be found [here](http://jse.amstat.org/v19n3/decock/DataDocumentation.txt)

### Business Recommendations
Based on our model, real estate agents can predict and propose price of property to home buyers using these features:

Neighborhood
Overall quality of the house
Size of the garage
Fireplaces
Total Number of rooms above ground
Fireplace quality
Age of house
Age of house remodelling
Gr Liv Area

While there are other analysis tool for agents to predict houses, those tools only allow selection of limited and basic features such as number of bed, type of house which you can normally expect. With our model, there are more features used to predict.

Agents may use our model as a complementary tool on top of other analysis tool such as Comparative Market Analysis (CMA) reports

**Limitations**
While this model generalizes well to the city of Ames, it's not generalizable to other cities, given that each city tends to differ greatly in terms of external factors like geographical features, seasonal weather or the economic climate of that particular city.

Another point to keep in mind that this model doesn't consider the inflation of housing prices. Since the end of the financial crisis in 2008, housing prices throughout the US have been increasing steadily year over year. Our model would need significant retraining to predict the current house prices in Ames today. 

Prices do not take into consideration of social factors (i.e. crime rates,  demographics in the neighborhood)

**Future project considerations:**
Feature importance - Provide coefficients of features to identify important features. 
Property survey portfolio: Property surveyor to evaluate the price of houses.
Extend to banks to establish the asset value of the houses