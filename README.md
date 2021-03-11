# Project 2

---
# Problem Statement
---

Intuitively we know there are several key aspects of a home that help to increase its selling price. We can assume the obvious: location, square footage, lot size, etc. But how can a home owner in Ames, IA looking to sell be certain the improvements they make will increase the sale price of their home?

Through the following data analysis, I will explore a substantial data set gathrered from the Ames, Iowa Assessor’s Office in attempt to focus in on key features of a home that can be upgraded to maximize sale price. 

I will first prepare and clean the data so it is ready for analysis. Then, I will perform some Exploratory Data Analysis in attempt to gleen some preliminary results. Finally, I will build and compare several different Linear Regression models, and choosing the most appropriate based on the R-squared and RMSE (root mean squared error) metrics. The model should provide solid quantitative power in determining target features of homes to upgrade.

---
# Data Dictionary
---

Data set contains information from the Ames Assessor’s Office used in computing assessed values for individual residential properties sold in Ames, IA from 2006 to 2010 ([source](http://jse.amstat.org/v19n3/decock/DataDocumentation.txt)). The original data come with an extremely verbose dictionary which can be referenced at the link below:

http://jse.amstat.org/v19n3/decock/DataDocumentation.txt

---
# Analysis
---

By using several different models: Linear Regression, cross validation, Ridge Regression and Lasso regression, it was determined the basic Linear Regression provided the best metrics in predicting home sale prices. The coefficients from this model were used in determing the key features that can be used for home owners to imporve and maximize the sale price of their homes. The final model has an R-squared value of 0.927 and a RMSE of 21405.38, which proved to be the best model.

---
# Conclusion
---

Our model showed there are some key areas home owners can improve in order to increase the sale price of their home in Ames, IA. The table below can be interpreted as every increase in a single unit from the feature column, the home seller can expect in increase in sale price equal to the coefficient (in dollars). For instance, assuming all other features are held constant, if the 'Overall Qual' of the home is increased by one grade, the seller can expect an $8,890 increase in sale price.

|**Feature**|**Coefficient (Dollar Increase in Sales Price**|
|---|---|
|Overall Qual|8990|
|Exterior Qual|7723|
|Kitchen Qual|7263|
|Garage Cars|7060|
|Fireplaces|3247|
|Total Rooms Above Ground|2017|
|Total Baths|1953|
|Has Garage|1915|
|Heating QC|1721|
|Paved Drive|1450|


The top three items are all related to the quality of the home: Overall, Exterior and Kitchen. The quality refers to the quality of finishes used in the hom: floors, tile, countertops, cabinets, molding, craftsmenship etc. These are mainly aesthetic features that can be modified relatively easily. The good thing are these provide the highest increase in sale price, as compared with something that will be highly unlikely to be modified such as with Garage Cars.

From the model, I highly recommend home owners focus on upgrading or renovating these key features:

    Overall Quality (+$8,990)
Exterior Quality (+$7,723)
    Kitchen Quality (+$7,263)
Heating QC (+$1,721)
    Paving the Driveway (+$1,450)
    
If major remodels are being planned, I urge them to consider updating the following features as the modeling suggests the are the strongest factors correlated with increasing sales prices:

    Increase in the number of cars a garage can accommodate (+$7,060)
Adding a fireplace (+$3,247)
    Adding a bathroom (+$1,953)
Adding a bedroom (+$2,017)

The future steps to move this project forward are trying to refine the modeling in order to better predict sale prices of higher priced homes. This in theory should have a trickle down effect of reducing the root mean squared error of all home price predictions, providing an overall better model.
 


```python

```
