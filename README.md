# MechaCar_Statistical_Analysis
## Linear Regression to Predict MPG
![linear_regression(1)](https://user-images.githubusercontent.com/33900637/156914158-9d093fb4-f2d2-43d4-b83c-a8cacca84a55.png)

### Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
From the dataset results it is possible to predict that the following variables/coefficients provided a non-random amount of variance to the mpg values:
vehicle weight(0.0776)
spoiler angle(0.3069)
AWD(All Wheel Drive)(0.1852)

### Is the slope of the linear model considered to be zero? Why or why not?
P-values (probability values) for the above variables are smaller than our significance level of 0.05. For example, the following is a calculation of the significance level for vehicle weight: 0.076 -1 = 0.9224 or 92.2%. The desired significance level is 0.05 - 1 = 0.95 or 95%). All 3 variable/coefficients are predicted to be outside the 95% minimum significance level based on the data used for the linear model. The intersept value (5.08e-08) in this model is statistically significant as well which means it is possibile other variables/coefficients may contribute to the variation in mpg that have not been included in our model (nor in the provided dataset). Additional values may still need to be collected or observed to increase the power of the analysis predeiction. The slope of the linear model is not considered to be zero because the p-value is less than 0.05.

### Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
According to the summary output, the r-squared value is 0.71, which predicts that approximatley 71% of all mpg predictions will be correct when using this linear model. In addition, the p-value of the linear model is 5.35e-11 (last line of the above picture in the F-statistic results), which is smaller (94.65%) than the desired significance level of 0.05 (95%).

## Create Visualizations for the Trip Analysis 
### The suspension coil’s PSI continuous variable across all manufacturing lots
### The following PSI metrics for each lot: mean, median, variance, and standard deviation.
##### Manufacturing Lot Summary
Below is the summary statistics of all of the manufacturing lots. The mean is 1498.78 for this sample and the population mean was determined to be 1500.

![total_lot_summary](https://user-images.githubusercontent.com/33900637/156914750-c2feade7-7211-4613-bda6-2e558a6b30cd.png)

##### Summary by Manufacturing Lot Number
The means of the lot numbers are similar to the population mean and the sample mean.
![manufactoring_lot_summary](https://user-images.githubusercontent.com/33900637/156914755-de85718d-34f5-41a8-bbec-9cdb726d0198.png)

## Summary Statistics on Suspension Coils
### The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
While the overall variance, as shown in the Total Summary data above, is under 100 psi and meets specifications, which is within the expected design specifications of staying under 100 PSI. However, there is a problem with one of the individual lots. When reviewing the data as shown in the Lot Summary stats, the variance for Lot 3 is well over the acceptable threshold, at 170.28. Thus, Lot 3 is a large contributing factor to the variance being high. 

## T-Tests on Suspension Coils
### summarize your interpretation and findings for the t-test results. Include screenshots of the t-test to support your summary.

## Study Design: MechaCar vs Competition
### Write a short description of a statistical study that can quantify how the MechaCar performs against the competition. In your study design, think critically about what metrics would be of interest to a consumer: for a few examples, cost, city or highway fuel efficiency, horse power, maintenance cost, or safety rating.
### In your description, address the following questions:
### What metric or metrics are you going to test?
### What is the null hypothesis or alternative hypothesis?
### What statistical test would you use to test the hypothesis? And why?
### What data is needed to run the statistical test?
