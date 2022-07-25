# Home-Market-Restraint
## Introduction
This project's objective is to forecast the selling price of a house, given the presence of specific qualities or attributes in that house.A model like this has many of useful applications in real life. For instance, a builder of new homes can decide on the ideal number of bedrooms, bathrooms, or a popular neighborhood to maximize selling price. This model could be used by a homeowner to choose the best asking price for their house. Alternately, a lender can use the model to estimate the worth of a house and then utilize that information to approve loans or set interest rates.
## Business Problem 
In the US, the number of homes has recently increased dramatically. The Zillow Home Value Index shows that prices increased by a startling 18% between 2020 and 2021. Now, purchasing a home in this market might bring in money for real estate investors. Real estate investors usually buy houses, fix them up, and resell them for a profit. Using a machine learning algorithm on previous data, the company will obtain a full understanding of the market 
## Problem statements
What is the potential cost of a new home?
Where in a certain County is it most advantageous to buy a new piece of property?
Is a home's renovation necessary?
What elements determine if a real estate investor wants to improve a house they recently purchased?
## Scope
The scope of the project is based on dataset with 20 variables
Identify relevant attributes
Data Preparation
Feature Selection/Feature Engineering
Exploratory Data Analysis
Data Visualization
Model Selection
Model Evaluation
Expected Results / Outcome
## EDA
Observation made from EDA Please see the appendix for the visualization

Price and number of bedrooms - A home's price rises as the number of bedrooms grows. With a little digging, we can find that there is only a $5K difference, but this is being stated without accounting for the impact of other amenities on price.
 
The relationship between price and bathrooms appears to be linear, thus when there are more bathrooms in a home, the price of the home also rises.

House price and interior square footage (sqft) - The price of the house rises as the interior square footage does. Their structure is linear.

Price and lot area(sqft) of the house** - Price and sqft_lot do not have any relationship. This feature doesn’t seem very predictive in determining house price.

Price and the Number of Floors in the House** - The cost of a home rises a little bit with the number of floors.

The cost and square footage (sqft) of the home. With each additional square foot of living space, the price of the home rises. Their structure is linear.

There is no correlation between the price and the basement's square footage (sqft). This function doesn't seem to be particularly accurate in predicting home prices.

The price of the house rises with the interior living space in square feet (sqft) for the 15 closest neighboring properties. Their structure is linear.

The price of the home and the average lot size of the 15 closest neighboring homes (in square feet) show no relationship. This function doesn't seem to be particularly accurate in predicting home prices.

The price of the home and the average lot size of the 15 closest neighboring homes (in square feet) show no relationship. This function doesn't seem to be particularly accurate in predicting home prices.

![image](https://user-images.githubusercontent.com/70611285/180699870-676573a9-e021-4f50-81cd-40d1dc97b6ef.png)

## Feature Engineering/Dimension Reduction
After the feature engineering we  have dropped the few variables which are not needed anymore and other variables are already been derived. to eventually determine which factors are connected with the price variable, a correlation chart is created. The graph demonstrates the strong correlation between price and attributes like square footage, bathrooms, and grade.
<img width="371" alt="image" src="https://user-images.githubusercontent.com/70611285/180699984-3031e625-2cbe-47f2-ad51-d0094c5942e3.png">
## Model Accuracy/Hyper tuning
After hyper tuning the Random Forest and fitting with the best estimator with MAE = 51,207
The model’s estimate is only $51K off from the actual worth of the house after the hyperparameters have been adjusted and tested on hypothetical data. Additionally, the model accounts for 86% of the price variation in the dataset.
![image](https://user-images.githubusercontent.com/70611285/180700051-2e81da0b-a93b-4160-aedf-2b5016f8bff8.png)
## Feature Importance
Not understanding which features contribute the most to the model makes no machine learning algorithm complete. We can see that factors like latitude and longitude, or the location of the home, the size of the interior living space, the home's quality and condition, and the typical size of a room, are crucial to consider when estimating the price of a home in King County. Real estate investors can pay close attention to these characteristics and determine how they connect to price before making selections about where to invest and where to spend their money.

![image](https://user-images.githubusercontent.com/70611285/180700099-8e1f5b4d-f3c5-4908-b3bd-1670aec0f3c1.png)

## Conclusion/Recommendation 
The best indicators of a home's price in King County are its location, its square footage of living space, its grade, and the size of its neighbors' houses taken together. The model can considerably assist real estate investors in taking all of these things into consideration when purchasing a home. The approach does, however, have a constraint in that it only applies to residences that cost less than $1,000,000 and typically have 2–6 bedrooms. Further research on this data revealed that the machine learning model creates significant residual errors since there is a lack of data on expensive residences.

## Future Uses/Additional Applications
On these data, four supervised machine learning models are being evaluated. In order to further reduce our mistake rate, we can try to utilize deep learning models like neural network models as our next step. Additionally, the algorithm can only anticipate homes under $1 million in value due to the lack of data on high-priced residences. We can get around this restriction by collecting more data, which can then be used to estimate pricey, high-priced homes.


