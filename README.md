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
#### Manufacturing Lot Summary
Below is the summary statistics of all of the manufacturing lots. The mean is 1498.78 for this sample and the population mean was determined to be 1500.

![total_lot_summary](https://user-images.githubusercontent.com/33900637/156914750-c2feade7-7211-4613-bda6-2e558a6b30cd.png)

#### Summary by Manufacturing Lot Number
The means of the lot numbers are similar to the population mean and the sample mean.
![manufactoring_lot_summary](https://user-images.githubusercontent.com/33900637/156914755-de85718d-34f5-41a8-bbec-9cdb726d0198.png)

## Summary Statistics on Suspension Coils
While the overall variance, as shown in the Total Summary data above, is under 100 psi and meets specifications, which is within the expected design specifications of staying under 100 PSI. However, there is a problem with one of the individual lots. When reviewing the data as shown in the Lot Summary stats, the variance for Lot 3 is well over the acceptable threshold, at 170.28. Thus, Lot 3 is a large contributing factor to the variance being high. 

## T-Tests on Suspension Coils
### T-Test for all Lots
<img width="512" alt="t_test_all" src="https://user-images.githubusercontent.com/33900637/156915280-1a416468-4684-4a78-a716-ba0c1a9960fd.png">
A review of the results of the T-Test for the suspension coils across all manufacturing lots shows that they are not statistically different from the population mean, and the p-value is not low enough (0.0603) for us to reject the null hypothesis.

### T-Test for Lot 1
<img width="556" alt="lot_1" src="https://user-images.githubusercontent.com/33900637/156915286-81da94a4-e5d7-48c0-9f43-a9e3571eb0af.png">
A review of the results of the T-test for the suspension coils for Lot 1 shows that they are not statistically different from the population mean, and the p-value is not low enough for us to reject the null hypothesis.

### T-Test for Lot 2
<img width="557" alt="lot_2" src="https://user-images.githubusercontent.com/33900637/156915289-8b3605df-1d23-4386-aa53-bda02ef84804.png">
A review of the results of the T-test for the suspension coils for Lot 2 shows that they are not statistically different from the population mean, and the p-value is not low enough for us to reject the null hypothesis.

### T-Test for Lot 3
<img width="556" alt="lot_3" src="https://user-images.githubusercontent.com/33900637/156915295-57375a2c-1633-441e-afc9-f5d0ab36f366.png">
A review of the results of the T-test for the suspension coils for Lot 3 shows that they are slightly statistically different from the population mean, and the p-value is just low enough for us to reject the null hypothesis. This lot may be need to be discarded, or at least more closely evaluated.

## Study Design: MechaCar vs Competition
In order to compare the performance of the MechaCar against the competition, we need to address a few observables which would be of interest to our customers. These variables will be cost, city and highway fuel efficiency, horsepower, safety rating, and carbon waste output.

We will be testing whether or not the MechaCar has statistically significant differences in these metrics compared to competing models. The null hypothesis will be that these observables don't vary significantly from the competition, and the alternative hypothesis will be that the MechaCar does indeed vary significantly in these variables compared to the competition.

We will perform one-tailed t-tests in order to determine if the MechaCar has higher or lower observed values in these variables than the competition according to which direction the consumer would prefer. The consumer would want the cost to be lower, the city and highway fuel efficiency to be higher, the horsepower to be higher, the safety rating to be higher, and the carbon waste output to be lower.

In order to run these statistical tests, we would need the cost, fuel efficiency, horsepower, safety rating, and carbon waste output data from the MechaCar as well as the MechaCar's competitors.
