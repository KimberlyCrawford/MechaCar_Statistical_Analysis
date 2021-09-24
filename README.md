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
- MechaCar MPG dataset
- Suspension Coil dataset

# Deliverable 1

The MechaCar_mpg.csv dataset contained mpg test results for 50 prototype MechaCars. The MechaCar prototypes were produced using multiple design specifications to identify ideal vehicle performance. Multiple metrics, such as vehicle length, vehicle weight, spoiler angle, drivetrain, and ground clearance, were collected for each vehicle. A linear model was designed that predicted the mpg of MechaCar prototypes using several variables from the MechaCar_mpg.csv file. 

## Linear Regression to Predict MPG

Below is a snapshot of the MechaCar MPG Dataset read as a dataframe:
![D1_MechaCar_mpg_dataframe.png](https://github.com/KimberlyCrawford/MechaCar_Statistical_Analysis/blob/main/Resources/Images/D1_MechaCar_mpg_dataframe.png)

Below is the linear regression performed using the lm() function to pass in all six variables (i.e., columns), and add the dataframe: 

![D1_Linear_Regression.png](https://github.com/KimberlyCrawford/MechaCar_Statistical_Analysis/blob/main/Resources/Images/D1_Linear_Regression.png)

Below is the summary that determined the p-value and the r-squared value for the linear regression model:

![D1_Summary.png](https://github.com/KimberlyCrawford/MechaCar_Statistical_Analysis/blob/main/Resources/Images/D1_Summary.png)

1) Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset? According to the below correlation results and table, vehicle_length has a positive 0.60947984 moderate correlation to mpg and ground_clearance has a positive 0.32874886 weak correlation to mpg while the other variables show very weak correlations. 

![D1_correlation.png](https://github.com/KimberlyCrawford/MechaCar_Statistical_Analysis/blob/main/Resources/Images/D1_correlation.png)
![D1_correlation_table.png](https://github.com/KimberlyCrawford/MechaCar_Statistical_Analysis/blob/main/Resources/Images/D1_correlation_table.png)

2) Is the slope of the linear model considered to be zero? Why or why not?
3) Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

# Deliverable 2
The MechaCar Suspension_Coil.csv dataset contains the results from multiple production lots. In this dataset, the weight capacities of multiple suspension coils were tested to determine if the manufacturing process is consistent across production lots. Using your knowledge of R, you’ll create a summary statistics table to show:

## Summary Statistics on Suspension Coils

![D2_Suspension_Coil.png](https://github.com/KimberlyCrawford/MechaCar_Statistical_Analysis/blob/main/Resources/Images/D2_Suspension_Coil.png)

![D2_Total_Summary_Suspension_Coil.png](https://github.com/KimberlyCrawford/MechaCar_Statistical_Analysis/blob/main/Resources/Images/D2_Total_Summary_Suspension_Coil.png)

![D2_Lot_Summary_Suspension_Coil.png](https://github.com/KimberlyCrawford/MechaCar_Statistical_Analysis/blob/main/Resources/Images/D2_Lot_Summary_Suspension_Coil.png)

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

# Deliverable 3

Using your knowledge of R, perform t-tests to determine if all manufacturing lots and each lot individually are statistically different from the population mean of 1,500 pounds per square inch.

## T-Tests on Suspension Coils

![D3_Sample_T_test.png](https://github.com/KimberlyCrawford/MechaCar_Statistical_Analysis/blob/main/Resources/Images/D3_Sample_T_test.png)

![D3_Lot_T-tests.png](https://github.com/KimberlyCrawford/MechaCar_Statistical_Analysis/blob/main/Resources/Images/D3_Lot_T-tests.png)

Briefly summarize your interpretation and findings for the t-test results. Include screenshots of the t-test to support your summary.

# Deliverable 4

Using your knowledge of R, design a statistical study to compare performance of the MechaCar vehicles against performance of vehicles from other manufacturers.

## Study Design: MechaCar vs Competition

Write a short description of a statistical study that can quantify how the MechaCar performs against the competition. In your study design, think critically about what metrics would be of interest to a consumer: for a few examples, cost, city or highway fuel efficiency, horse power, maintenance cost, or safety rating.
In your description, address the following questions:
What metric or metrics are you going to test?
What is the null hypothesis or alternative hypothesis?
What statistical test would you use to test the hypothesis? And why?
What data is needed to run the statistical test?