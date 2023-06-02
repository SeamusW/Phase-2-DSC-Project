![image](https://github.com/SeamusW/Phase-2-DSC-Project/assets/32468677/53544128-e77e-4368-ae5f-492f54a53bc4)


# Phase-2-DSC-Project
# Analysis of King County Real Estate

*Seamus Walsh and Daniel Gieseke | June 2, 2023*

## Overview
King County, Washington boasts a dynamic real estate market with a variety of homes.  With this project we took in data on homes sold within King County to understand which home features affect sale price.  We not only included data from homes sold in the county, but included data on population, income, and geographic distances from select county features.  Our aim with this project is to create a predictive model that will tell potential home buyers or home value assesors a predicted value of a home based on select features of a home.

## Project and Data Links
<a href="https://github.com/SeamusW/Phase-2-DSC-Project/blob/main/King%20County%20Housing%20Data%20Exploratory%20Data%20Analysis.ipynb">Main Project File</a>

<a href="TBD">Project Slide Deck</a>

<a href="https://github.com/learn-co-curriculum/dsc-phase-2-project-v2-5/tree/main/data">Data Source: King County Housing Data</a>

<a href="https://www.point2homes.com/US/Neighborhood/WA/King-County-Demographics.html">Data Source: US Census Bureau Data via Point2Homes.com</a>

## Business Understanding
There are several factors that contribute to home prices:
<ul>
  <li>Square footage (outdoor/indoor, above/below ground), amount of bed/bathrooms, quality of the home, age of the home, price of the neighboring homes, etc.
  <li>Using various sources, we've provided several data-driven strategies to compare your home to what it's expected value should be.
</ul>

## Data Understanding
Our data sources included King County Housing Data, including information on over 32,000 homes sold in King County, Washington. We also used data from the US Census Bureau (via Point2Homes.com). Altogether, this included information on home price, sell date, square footage, beds/bathrooms, views, address, outdoor space, income, population, and much more.


## Data Analysis
For our analysis we sought to understand the best predictors of home prices based on all of these data points. 
    
## Baseline Model
Our baseline model started with looking simply at the relationship between square footage and home price. We decided on square footage as our baseline model because it was the most highly correlated variable to price.
![image](https://github.com/SeamusW/Phase-2-DSC-Project/assets/32468677/eb37e592-8483-401e-a3b6-e9b141572445)


    
![image](https://github.com/SeamusW/Phase-2-DSC-Project/assets/32468677/10d410a2-8495-44be-965b-6feeca4bd121)

    
![image](https://github.com/SeamusW/Phase-2-DSC-Project/assets/32468677/21ceda31-133d-4272-b8d2-b0e5e4622d24)

This baseline model had an adjusted R-sqaure of .406 and a Mean Absolute Error of 338783.
    
## Secondary Model
Next, we added more variables into our model that also showed correlations with overal home price.
![image](https://github.com/SeamusW/Phase-2-DSC-Project/assets/32468677/e0b63e82-57be-4349-8b7a-114566451af2)

This model increased our adjusted R-square to .466 and reduced the Mean Absolute Error to 320281.
    
## Final Model
The final model included feature engineered variables based on the results we got from our previous models. Specifically, we looked at interactions between zip codes and average home price, zip codes and average income, sqaure footage and condition of the home, as well as the distance from the fastest growing areas of King County.
![image](https://github.com/SeamusW/Phase-2-DSC-Project/assets/32468677/e39c81a3-64a3-42d5-bce9-476b00c75c1d)
![image](https://github.com/SeamusW/Phase-2-DSC-Project/assets/32468677/d845592b-6c24-433c-90f9-9af7c6e6e128)
    
This final model increased our adjusted R-square to .767 and reduced the Mean Absolute Error to 187397.
Meaning, this model accounts for approximately 77% of the variance in Price, and can accurately predict a housing price within $187,397 dollars.

## Recommendations and Features to Consider
There are a number of features that affect a home's sale price with several that are common sense including the square footage and condition, of a home.  A few key features we found interesting that we suggest home value assessors and potential buyers to consider are as follows.
<ul>
<li>Distance from Bellevue and Kirkland
<ul><li>Our model shows that your distance from Kirkland and Bellevue affects your home price.  Increasing your proximity to these cities increases your home sale price.</ul>
  
<li>Whole Foods in Your Zip Code
<ul><li>Our model shows that if a Whole Foods is in your home’s zip code, your home sale price increases.</ul>

<li>Median Sale Price of Other Homes in Your Zip Code
<ul><li>Our model shows that the higher the median sale price of other homes in your zip code affects your home price.  Unsurprisingly, as the sale price as other homes in your zip code increases, so does your home price.</ul>
</ul>

## Next Steps
Potential next steps for this project could include sourcing additional data that is missing from our current data set and running additional tests with regression model.

## Repository Structure
Daniel folder This folder houses Daniel's working documents.

Seamus folder This folder houses Seamus's working documents.

Exploring Movie Data Project - Slide Deck This file is a slide deck covering our analysis.

King County Housing Data Exploratory Data Analysis - This file contains our data cleaning and wrangling, as well as all of our models and visualizations.

Testing the Model - This file contains the predictive testing of our final model.
    
README.md This is the file you are reading now that gives an overview of our project
