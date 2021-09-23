# MechaCar_Statistical_Analysis

# Overview
AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on Jeremy and the data analytics team to review the production data for insights that may help the manufacturing team.

## Purpose
In this challenge, you’ll help Jeremy and the data analytics team do the following:

- Deliverable 1: Linear Regression to Predict MPG - Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes
- Deliverable 2: Summary Statistics on Suspension Coils - Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
- Deliverable 3: T-Test on Suspension Coils - Run t-tests to determine if the manufacturing lots are statistically different from the mean population
- Deliverable 4: Design a Study Comparing the MechaCar to the Competition - Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.

## Resources
- MechaCar MPG dataset
- Suspension Coil dataset

### Deliverable 1 Instructions

The MechaCar_mpg.csv dataset contains mpg test results for 50 prototype MechaCars. The MechaCar prototypes were produced using multiple design specifications to identify ideal vehicle performance. Multiple metrics, such as vehicle length, vehicle weight, spoiler angle, drivetrain, and ground clearance, were collected for each vehicle. Using your knowledge of R, you’ll design a linear model that predicts the mpg of MechaCar prototypes using several variables from the MechaCar_mpg.csv file. Then, you’ll write a short interpretation of the multiple linear regression results in the README.md.

## Linear Regression to Predict MPG

![D1_Linear_Regression.png](https://github.com/KimberlyCrawford/MechaCar_Statistical_Analysis/blob/main/Resources/Images/D1_Linear_Regression.png)

![D1_MechaCar_mpg_dataframe.png](https://github.com/KimberlyCrawford/MechaCar_Statistical_Analysis/blob/main/Resources/Images/D1_MechaCar_mpg_dataframe.png)

![D1_Summary.png](https://github.com/KimberlyCrawford/MechaCar_Statistical_Analysis/blob/main/Resources/Images/D1_Summary.png)


1) Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
2) Is the slope of the linear model considered to be zero? Why or why not?
3) Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

### Deliverable 2 Instructions
The MechaCar Suspension_Coil.csv dataset contains the results from multiple production lots. In this dataset, the weight capacities of multiple suspension coils were tested to determine if the manufacturing process is consistent across production lots. Using your knowledge of R, you’ll create a summary statistics table to show:

The suspension coil’s PSI continuous variable across all manufacturing lots
The following PSI metrics for each lot: mean, median, variance, and standard deviation.
Then, in the README.md, you’ll briefly detail and interpret the suspension coil summary statistics.

## Summary Statistics on Suspension Coils

![D2_Suspension_Coil.png](https://github.com/KimberlyCrawford/MechaCar_Statistical_Analysis/blob/main/Resources/Images/D2_Suspension_Coil.png)

![D2_Total_Summary_Suspension_Coil.png](https://github.com/KimberlyCrawford/MechaCar_Statistical_Analysis/blob/main/Resources/Images/D2_Total_Summary_Suspension_Coil.png)

![D2_Lot_Summary_Suspension_Coil.png](https://github.com/KimberlyCrawford/MechaCar_Statistical_Analysis/blob/main/Resources/Images/D2_Lot_Summary_Suspension_Coil.png)

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

### Deliverable 3 Instructions
Using your knowledge of R, perform t-tests to determine if all manufacturing lots and each lot individually are statistically different from the population mean of 1,500 pounds per square inch.

## T-Tests on Suspension Coils

briefly summarize your interpretation and findings for the t-test results. Include screenshots of the t-test to support your summary.


### Deliverable 4 Instructions

Using your knowledge of R, design a statistical study to compare performance of the MechaCar vehicles against performance of vehicles from other manufacturers.

## Study Design: MechaCar vs Competition

Write a short description of a statistical study that can quantify how the MechaCar performs against the competition. In your study design, think critically about what metrics would be of interest to a consumer: for a few examples, cost, city or highway fuel efficiency, horse power, maintenance cost, or safety rating.
In your description, address the following questions:
What metric or metrics are you going to test?
What is the null hypothesis or alternative hypothesis?
What statistical test would you use to test the hypothesis? And why?
What data is needed to run the statistical test?