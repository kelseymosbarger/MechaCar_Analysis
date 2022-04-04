# MechaCar_Analysis
Module 15

## Overview
The goal of this analysis is to perform the following list for AutosRUs:
- Linear regression model to predict MGP
- Summary statistics on suspension coils
- T-Test on suspension coils
- Design a study compairinf the MechaCar to competitor

#### Resources
R, RStudio, Data from Module


## Results

### Linear Regression to Predict MPG

<table><tr><td>
 
<tr><td>#### Which variables/coeeficients provided a non-random amount of varaiance to the mpg values in the dataset?</td></tr>

![image](https://user-images.githubusercontent.com/94019661/161610216-1847361b-c78b-4340-b2b3-24f0cc352c53.png)

<table><tr><td> vehicle_length and ground_clearance followed by vehicle_weight are the variables with a non-random amount of variance to the mpg values.</td></tr></table> 
 
</td></tr></table> 


<table><tr><td>
 
#### is the Slope on the linear model considered to be zero? why or why not?


![image](https://user-images.githubusercontent.com/94019661/161610233-22296f60-fa94-46b5-8b77-1857b0a53b79.png)

<table><tr><td> The slope of the linear model is not cosidered to be zero, 
 becuase the P-value is considerably less than the significance level of 0.05%. 
 In this case it is safe to reject the null hypothesis.</td></tr></table> 
 
</td></tr></table> 



<table><tr><td>
 
#### Does this linear model predict mpg of MechaCar prototypes effectively? why or why not?


<table><tr><td> The linear model predicts that 71% of MPG estimates are correct using this
 model. There is a strong correlation between MPG and the 5 variables. It would depend if 
 71% probablity of accuracy is enough. </td></tr></table> 
 
</td></tr></table> 




### Summary Statistics on Suspension Coils


<table><tr><td>
 
#### The design specifications for the MechaCar suspension coils dictate that the variance 
of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing 
data meet this design specification for all manufacturing lots in total and each lot individually? 
 Why or why not?

![image](https://user-images.githubusercontent.com/94019661/161610293-647f02d9-7deb-4b0e-9ee3-3424017538ac.png)

<table><tr><td> Looking at the total_summary, you can see that the variance of the suspension coils for all of the lots is 62.29. This view of the data is within the 100 PSI max MechaCar design specifications. </td></tr></table> 

![image](https://user-images.githubusercontent.com/94019661/161610323-47e53d0d-5a37-48c3-9860-d9da0956dbfc.png)

<table><tr><td> When you cohort the data by manufacturing lot, lots 1 and 2 fall within MechaCar's design specifications. However, as you can see with Lot 3 - the variance is ~170 which far exceeds the design specs for MechaCar.</td></tr></table> 
 
</td></tr></table> 



### T-Tests on Suspension Coils


<table><tr><td>
 
#### summary of T-Test results.

![image](https://user-images.githubusercontent.com/94019661/161610351-3071c991-6f44-4276-ba91-3798ae756211.png)

<table><tr><td> T-Test for all manufacturing lots for suspension coils has a p-value of 0.6, and the mean is 1498.78 vs 1500. The p-value indicates that the mean vs the population mean are statistically similar since it is above the 0.05 significance level.</td></tr></table> 


![image](https://user-images.githubusercontent.com/94019661/161610371-f1b5c017-0a73-436b-b93f-22c2389644b8.png)

![image](https://user-images.githubusercontent.com/94019661/161610382-47c4a0fc-dd79-4ec5-8aeb-ebe40dde6fbf.png)

![image](https://user-images.githubusercontent.com/94019661/161610399-7d6efac4-c2d4-4e05-ab28-e10366ceb123.png)


<table><tr><td> When analyzing the t-test by maufacturing lot. Lots 1 and 2 are not statistically different enough to reject the null hypothesis. However, Lot 3, with a mean of 1496.14 and p-value of 0.042 which is under the significance level tells us that Lot 3 suspension coils are statistically different from the population mean.</td></tr></table> 
 
</td></tr></table> 



## Study Design: MechaCar vs Competition

How does MechaCar stand up against the competition? Additional analysis to ensure that MechaCar holds a competitive advantage in the marketplace.


<table><tr><td>
 
#### Metric to be Tested


<table><tr><td> One very important factor in car buying that should additionally be considered is the cost of a MechaCar and how that stacks up to the competition. As well as how well the car hold it's value over time compared to the competition.</td></tr></table> 


#### What is the null hypothesis or alternative hypothesis?**

 <table><tr><td>  **Null Hypothesis :
  The mean price/cost of car is the same across all car brands

  **Alternative Hypothesis :
  At least one Car in the dataset has a different mean cost/price than the other cars.</td></tr></table> 


#### What statistical test would you use to test the hypothesis? And why?

<table><tr><td> First would start with a paired t-test to get the p-value which then we can compare to the significance level. As well as see the range in the difference of means to gauge where MechaCar lands in the mix.</td></tr></table> 


#### Data Required

<table><tr><td> Additional analysis would be to run some linear regression on MechaCar and competitors to see if there are any very strong correlation in price of car to the features in the car and see if there are any trends that are industry wide or if it is brand specific.

You would need data on competing cars, including the information that was provided in the module and a cost dataset. You would probably want to include ~300 car dataset to get a full picture of the copmpetitive landscape.

Redisual/resale value would be harder to measure as there is much more variability that goes into selling a used car, but nonetheless would be an interesting sales point.</td></tr></table> 
 
</td></tr></table> 

