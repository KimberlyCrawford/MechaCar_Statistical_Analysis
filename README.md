# MechaCar_Statistical_Analysis

# Overview
AutosRUs’ newest prototype, the MechaCar, was suffering from production troubles that were blocking the manufacturing team’s progress. AutosRUs’ upper management called on Jeremy and the data analytics team to review the production data for insights that may help the manufacturing team.

## Purpose
The purpose of this analysis was to complete the following deliverables:

- Deliverable 1: Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes.
- Deliverable 2: Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots.
- Deliverable 3: Run t-tests to determine if the manufacturing lots are statistically different from the mean population.
- Deliverable 4: Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. 

## Resources
- MechaCar MPG dataset with 50 observations and 6 variables
- Suspension Coil dataset

## Statistical Notes

- If the p-value is greater than 0.05, the data is considered normally distributed. Remember that most basic statistical tests assume an approximate normal distribution. Therefore, if our p-value is around 0.05 or more, we would say that our input data meets this assumption. But what happens if our data distribution does not look like a bell curve, or the p-value of the Shapiro-Wilk tests is too small?
- A multiple linear regression uses multiple independent variables to account for parts of the total variance observed in the dependent variable.


## Deliverable 1

The MechaCar_mpg.csv dataset contained mpg test results for 50 prototype MechaCars. The MechaCar prototypes were produced using multiple design specifications to identify ideal vehicle performance. Multiple metrics, such as vehicle length, vehicle weight, spoiler angle, drivetrain, and ground clearance, were collected for each vehicle. A linear model was designed that predicted the mpg of MechaCar prototypes using several variables from the MechaCar_mpg.csv file. 

### Linear Regression to Predict MPG

Below is a snapshot of the MechaCar MPG Dataset read as a dataframe:

![D1_MechaCar_mpg_dataframe.png](https://github.com/KimberlyCrawford/MechaCar_Statistical_Analysis/blob/main/Resources/Images/D1_MechaCar_mpg_dataframe.png)

Below is the linear regression performed using the lm() function to pass in all six variables (i.e., columns), and add the dataframe. The first five variables (vehicle length, vehicle weight, spoiler angle, AWD, and ground clearance) in the dataset are the independent variables while the last variable (mpg) is the dependent variable. 

![D1_Linear_Regression.png](https://github.com/KimberlyCrawford/MechaCar_Statistical_Analysis/blob/main/Resources/Images/D1_Linear_Regression.png)

Below is the summary that determined the p-value and the r-squared value for the linear regression model:

![D1_Summary.png](https://github.com/KimberlyCrawford/MechaCar_Statistical_Analysis/blob/main/Resources/Images/D1_Summary.png)

1) Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset? In the summary output, each Pr(>|t|) value represents the probability that each coefficient contributes a random amount of variance to the linear model. According to our results, vehicle length and ground clearance (as well as intercept) are statistically unlikely to provide random amounts of variance to the linear model.

The below correlation results and table show vehicle_length has a positive 0.60947984 moderate correlation to mpg and ground_clearance has a positive 0.32874886 weak correlation to mpg while the other variables show very weak correlations. 

![D1_correlation.png](https://github.com/KimberlyCrawford/MechaCar_Statistical_Analysis/blob/main/Resources/Images/D1_correlation.png)
![D1_correlation_table.png](https://github.com/KimberlyCrawford/MechaCar_Statistical_Analysis/blob/main/Resources/Images/D1_correlation_table.png)

2) Is the slope of the linear model considered to be zero? Why or why not? No, the p-value is 5.35e-11 which is smaller than the assumed significance level of 0.05. Therefore, we can state that there is sufficient evidence to reject our null hypothesis, which means that the slope of our linear model is not zero. 

3) Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?  Yes, the r-squared value is 0.7149 which means 71% of the data fit the regression model. Generally, a higher r-squared indicates a better fit for the model.

## Deliverable 2

The MechaCar Suspension_Coil.csv dataset contains the results from multiple production lots. In this dataset, the weight capacities of multiple suspension coils were tested to determine if the manufacturing process is consistent across production lots. 

### Summary Statistics on Suspension Coils

![D2_Suspension_Coil.png](https://github.com/KimberlyCrawford/MechaCar_Statistical_Analysis/blob/main/Resources/Images/D2_Suspension_Coil.png)

![D2_Total_Summary_Suspension_Coil.png](https://github.com/KimberlyCrawford/MechaCar_Statistical_Analysis/blob/main/Resources/Images/D2_Total_Summary_Suspension_Coil.png)

![D2_Lot_Summary_Suspension_Coil.png](https://github.com/KimberlyCrawford/MechaCar_Statistical_Analysis/blob/main/Resources/Images/D2_Lot_Summary_Suspension_Coil.png)

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. The current manufacturing data does meet this design specification for all manufacturing lots in total (variance 62.29356); however, Lot 3 does not meet the design spec with a variance of 170.2861224.

## Deliverable 3

T-tests were performed to determine if all manufacturing lots and each lot individually are statistically different from the population mean of 1,500 pounds per square inch.

### T-Tests on Suspension Coils

Assuming our significance level was the common 0.05 percent, our p-value was above our significance level. Therefore, we do not have sufficient evidence to reject the null hypothesis; the two means are statistically similar.

![D3_Sample_T_test.png](https://github.com/KimberlyCrawford/MechaCar_Statistical_Analysis/blob/main/Resources/Images/D3_Sample_T_test.png)

Assuming our significance level was the common 0.05 percent, our p-value was above our significance level for Lots 1 and 2. Therefore, we do not have sufficient evidence to reject the null hypothesis; the two means are statistically similar. Since the p-value for Lot 3 was lower than the significance level, we have sufficient evidence to reject the null hypothesis; the two means are statistically different.

![D3_Lot_T-tests.png](https://github.com/KimberlyCrawford/MechaCar_Statistical_Analysis/blob/main/Resources/Images/D3_Lot_T-tests.png)

## Deliverable 4

Using your knowledge of R, design a statistical study to compare performance of the MechaCar vehicles against performance of vehicles from other manufacturers.

### Study Design: MechaCar vs Competition

A study to test MechaCar against the competition might include the following:

- Metric or metrics being tested: Consumer rating, cost, fuel efficiency, and vehicle class.
- Null hypothesis or alternative hypothesis: H0: There is NO statistical significant difference on defined metrics between MechaCar and competition. Ha: The is statistical significant difference on defined metrics between MecharCar and competition.
- Statistical test used to test the hypothesis and reason selected this test: t-tests on each metrics for MechaCar against the same metric from the collective competition data.
- Data needed to run the statistical test: Consumer rating, cost, fuel efficiency, and vehicle class.