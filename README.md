
## Project Overview
This project aims to provide valuable insights for a realtor operating in King County, Washington, USA. Specifically, the agency seeks to provide accurate estimates on how to conduct extensive research on the real estate market in King County in order to determine the variables that affect house pricing, and factors that affect house grade and identify areas of spatial clustering based on price. This approach can help homeowners to add functionality to their property while simultaneously boosting the value. These details will help the agency guide their clients and alternatively use the information towards making informed decisions on home renovations, which can maximize their return on investment when selling their properties.

## Business Problem
As we can see the industry is very lucrative but also has the ability to cause great losses when house pricing gets out of control. This means that potential investors have to make smart and informed decisions so as to safeguard their money, they want to get maximum value, no matter how much is spent. After all who likes to be known to make poor investment decisions and what better way to ensure this than with data-driven decisions. In order to achieve this they will consider both simple and multiple linear regression models to analyze house sales data in the King County area.

### Business and Data Understanding
Real estate is a physical asset with the potential to appreciate in value over time. In fact, historical data shows that real estate appreciates at a higher rate than the rate of inflation. This means that over time, the value of your property will increase, which can lead to significant profits. To help our stakeholders KC Real Estate Agency seeks to use a data-driven insight
How do we go about ensuring that this real estate agency gets the most out of its money? We've set the following objectives to help guide:

**1. To determine which variables affect house pricing, more specifically those that increase the value of a house.**

**2. Factors that affect grade of a house. We want to invest in only high grade houses despite the price.**

**3. To identify similar areas of spatial clustering based on the price.** 

### The Data

This project uses the King County House Sales dataset, which can be found in  `kc_house_data.csv`. The columns are as below:
The aspects we will be examining are as follows to determine correlations based on the objective:

1 price - sales price

2 bedrooms - Number of bedrooms

3 bathrooms - Number of bathrooms

4 sqft_living - Square footage of living space in the home

5 sqft_lot - Square footage of the lot

6 floors - Number of floors (levels) in house

7 waterfront - whether the house is on a waterfront

8 grade - Overall grade of the house. Related to the construction and design of the house

9 yr_built - Year when house was built

10 condition - How good the overall condition of the house is. Related to the maintenance of house

# #Rationale

By opting for statistical analyses over basic data visualization, we are aiming to gain a deeper insight into the relationships within our data. While graphs offer a visual representation, regression coefficients offer precise measurements of the influence each feature has on house prices and how they can affect the grade. This level of granularity is crucial in the intricate domain of real estate, where numerous factors come together to determine property values. Through regression analysis, we can uncover subtle effects and segmentation of house prices, providing a thorough evaluation for our audience in the field of data science. These statistical insights guided our modeling process, ultimately ensuring the accuracy and effectiveness of our model.

## Modeling and Regression Results**
##### Objective 1
For our first model, we checked how sqft_above and sqft_living affect price

![image](https://github.com/MugoDom/dsc-phase-2-project-v2-3/assets/133999173/2488e48c-67d9-4dd5-b7e6-24b0ac502091)



#### Objective 2
In the second model, we checked the correlation between the dependent and independent variables

<img width="570" alt="Objective2" src="https://github.com/MugoDom/dsc-phase-2-project-v2-3/assets/133999173/db12a6b4-e351-4b55-b0b3-2f26e2bde7a1">


#### Objective 3
The third model seeks to identify areas of similar spatial clustering based on house prices 
![image](https://github.com/MugoDom/dsc-phase-2-project-v2-3/assets/133999173/a9e8efd2-802d-45da-a099-9a87879d37e7)



## Conclusions

1.sqft_living and sqft_above independent variables are statistically significant in determining the dependent variable price. sqft_living explains 49.6% of the variance in price and sqft_above explains 37.1% of the variance in price. Hence the realtor might consider taking the sqft_living and sqft_above as determinants of fixing the value of the house in regard to price.

The grade of a house of a house has a high correlation with the size of the living room, square footage of the house apart from the basement, and price. This should be put under consideration if the intention is only on high-grade houses for profit maximization.

These clusters may be helpful to investors in locating possible investment possibilities. Investment opportunities in inexpensive housing may exist in Cluster 0, whilst luxury real estate may be sought after in Cluster 1 meaning considerations should be on Cluster 1.
## Next steps
1. Now that we know the factors that affect the price and grade of a house, the follow-up step is to find which areas have external 
developments(malls, developed roads) that would make people want to buy homes there.
2. Observe areas where a lot of people are moving and find ways in which the real estate agency can invest there.
3. To collect further parameters that may affect the price and grade of a house in order to make adjustments on the R-squared.

