# Phase-2-DSC-Project
# Analysis of King County Real Estate

*Seamus Walsh and Daniel Gieseke | June 2, 2023*

## Overview


## Project and Data Links


## Business Understanding
There are several factors that contribute to home prices:
<ul>
  <li>Square footage (outdoor/indoor, above/below ground), amount of bed/bathrooms, quality of the home, age of the home, price of the neighboring homes, etc.
  <li>Using various sources, we've provided several data-driven strategies to compare your home to what it's expected value should be.


## Data Understanding
Our data sources included King County Housing Data, including information on over 32,000 homes sold in King County, Washington. We also used data from the US Census Bureau (via Point2Homes.com). Altogether, this included information on home price, sell date, square footage, beds/bathrooms, views, address, outdoor space, income, population, and much more.


## Data Analysis
For our analysis we sought to understand the best predictors of home prices based on all of these data points. 
    
## Baseline Model
Our baseline model started with looking simply at the relationship between square footage and home price. We decided on square footage as our baseline model because it was the most highly correlated variable to price.
    
This baseline model had an adjusted R-sqaure of .406 and a Mean Absolute Error of 338783.
    
## Secondary Model
Next, we added more variables into our model that also showed correlations with overal home price.
    

This model increased our adjusted R-square to .466 and reduced the Mean Absolute Error to 320281.
    
## Final Model
The final model included feature engineered variables based on the results we got from our previous models. Specifically, we looked at interactions between zip codes and average home price, zip codes and average income, sqaure footage and condition of the home, as well as the distance from the fastest growing areas of King County.
    
    
This final model increased our adjusted R-square to .767 and reduced the Mean Absolute Error to 187397.
Meaning, this model accounts for approximately 77% of the variance in Price, and can accurately predict a housing price within $187,397 dollars.

## Recommendations


## Next Steps


## Repository Structure

