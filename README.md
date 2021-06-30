# MechaCar_Statistical_Analysis

## Project Overview

## Resources
*  Data Source: MechaCar_mpg.csv, Suspension_coil.csv
*  Software: RStudio

## Linear Regression to Preditct MPG
•	Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

        Based on the summary of linear Regression, vehicle length and ground clearance provided a non-random amount of variance to the mpg values in the dataset by their low p-values result.

•   Is the slope of the linear model considered to be zero? Why or why not?

        The p-Value for this model is much smaller than the assumed significance level of 0.05%. This indicates there is sufficient evidence to reject our null hypothesis, which further indcates that the slope of this linear model is not zero.

•   Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
    
        The linear model has an r-squared value of 0.7149, which means that this model predicts the mpg of MechaCar protoypes effectively 

## Summary Statistics on Suspension Coils
•   The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 
    pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and   each lot individually? Why or why not?

        The MechaCar suspension coils specs variance to not to exceed to 100. The table below shows that over all variance of the coils is within the 100 PSI variance requirement. However, Lot3 variance is over the 100 PSI variance requirement

## T-Test on Suspension Coils
   
### T-test all manufacturing lots agains the population mean
    Assuming our significance level is the common 0.05 percent, our p-value of 0.060 is above the significance level. Therefore, we do not have sufficient evidence to reject the null hypothesis, and we can state that the PSI across all manufacturing lots is statiscally similar to the population mean of 1498.78 psi.

### T-Tests each manufacturing lot against the population mean

    Lot1 The results of the t-test to test if the PSI mean for Lot1 is statistically different from the population mean of 1,500 pounds per square inch show that, at a 95% confidence level, the two means are not statistically different. The p-value of 1 shows that the mean for Lot1 is exactly the same same as the population mean of 1500 PSI.

    Lot2 The results of the t-test to test if the PSI mean for Lot2 is statistically different from the population mean of 1,500 pounds per square inch show that, at a 95% confidence level, the two means are not statistically different. Because the p-value of 0.6072 is higher than the critical value of 0.05, the null hypothesis can be accepted in that there is no difference between the means of the PSI for the population and Lot2. 

    Lot3 The results of the t-test to test if the PSI mean for Lot3 is statistically different from the population mean of 1,500 pounds per square inch show that, at a 95% confidence level, the two means are statistically different. Because the p-value of 0.04168 is lower than the critical value of 0.05, the null hypothesis should be rejected in that there is a difference between the means of the PSI for the population and Lot3 and the true mean is not equal to 1500. The means within the 95% confidence range are between 1492.431 and 1499.849 PSI.

## Study Design: MechaCar vs. Competition

The cost of owning and maintaining a vehicle can be expensive, so AutosRUs wants to make sure their customers are getting the best value over their competitors and would like to measure the rate of depreciation for MechaCars against other manufacturers.

-   Metric - Rate of depreciation (value of vehicle over time)

-   Hypothesis -
        Null hypothesis: Rate of depreciation for MechaCars is equal to their competitors
        Alternative hypothesis: Rate of depreciation for MechaCars is not equal to their competitors

-   Statistical Test -  use multiple linear regression to predict MechaCar's rate of depreciation

-   Data - vehicle value , how old is the vehicle and mileage.
