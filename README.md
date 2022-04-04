# MechaCar_Analysis
Module 15

## Overview
The goal of this analysis is to perform the following list for AutosRUs:
- Linear regression model to predict MGP
- Summary statistics on suspension coils
- T-Test on suspension coils
- Design a study compairinf the MechaCar to competitor

#### Resources
R, RStudio
Data from Module


## Results
### Linear Regression to Predict MPG

- which variables/coeeficients provided a non-random amount of caraiance to the mpg values in the dataset?

Screenshot***

vehicle_length and ground_clearance followed by vehicle_weight are the variables with a non-random amount of variance to the mpg values. 

- is the Slope on the linear model condiered to be zero? why or why not?

Screenshot

The slope of the linear model is not cosidered to be zero, becuase the P-value is considerably less than the significance level of 0.05%. In this case it is safe to reject he null hypothesis.

- Does this linear model predict mpg of MechaCar prototypes effectively? why or why not?

The linear model predicts that 71% of MPG estimates are correct using this model. There is a strong correlation between MPG and the 5 variables. It would depend if being 71% probablity of accuracy is enough. 


### Summary Statistics on Suspension Coils

- The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

screenshot total_summary image (with summary of it)

Looking at the total_summary, you can see that the variance of the suspension coils for all of the lots is 62.29. This view of the data is within the 100 PSI max MechaCar design specifications. 

screenshot lot_summary image (with summary of it)

When you cohort the data by manufacturing lot, lots 1 and 2 fall within MechaCar's design specifications. However, as you can see with Lot 3 - the variance is ~170 which far exceeds the design specs for MechaCar.


### T-Tests on Suspension Coils

- summary of T-Test results.

Screenshot

T-Test for all manufacturing lots for suspension coils has a p-value of 0.6, and the mean is 1498.78 vs 1500. The p-value indicates that the mean vs the population mean are statistically similar since it is above the 0.05 significance level.

Screenshot

Screenshot

Screenshot

When analyzing the t-test by maufacturing lot. Lots 1 and 2 are not statistically different enough to reject the null hypothesis. However, Lot 3, with a mean of 1496.14 and p-value of 0.042 which is under the significance level tells us that Lot 3 suspension coils are statistically different from teh population mean.


## Study Design: MechaCar vs Competition

How does MechaCar stand up against the competition? Additional analysis to ensure that MechaCar holds a competutive advantage in the marketplace.

- Cost Analysis

One very important factor in car buying that should additionally be considered is the cost of a MechaCar and how that stacks up to the competition. As well as how well the car hold it's value over time compared to the competition.

- What is the null hypothesis or alternative hypothesis?

Null Hypothesis : The mean price/cost of car is the same across all car brends
Alternative Hypothesis : The mean price/cost of car is 

- What statistical test would you use to test the hypothesis? And why?
First would start with a paired t-test to get the p-value which then we can compare to the significance level. As well as see the range in the difference of means to gauge where MechaCar lands in the mix.

Additional analysis would be to run some linear regression on MechaCar and competitors to see if there are any very strong correlation in price of car to the features in the car and see if there are any trends that are industry wide or if it is brand specific.

You would need data on competing cars, including the information that was provided in the module and a cost dataset. You would probably want to include ~300 car dataset to get a full picture of the copmpetitive landscape.

Redisual/resale value would be harder to measure as there is much more variability that goes into selling a used car, but nonetheless would be an interesting sales point.

