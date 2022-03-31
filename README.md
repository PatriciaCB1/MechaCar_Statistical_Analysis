# MechaCar_Statistical_Analysis

## Overview of the project
AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. Upper management has called the data analytics team to review the production data for insights that may help the manufacturing team.

Objectives:

- Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes
- Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
- Run t-tests to determine if the manufacturing lots are statistically different from the mean population
- Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.

This project consists of three technical analysis deliverables and a proposal for further statistical study as follows:

Deliverable 1: Linear Regression to Predict MPG
Deliverable 2: Summary Statistics on Suspension Coils
Deliverable 3: T-Test on Suspension Coils
Deliverable 4: Design a Study Comparing the MechaCar to the Competition

## Resources
Software: R version 4.0.1
Data:  MechaCar_mpg.csv, Suspension_Coil.csv

## Linear Regression to Predict MPG
The MechaCar_mpg.csv dataset contains mpg test results for 50 prototype MechaCars. The MechaCar prototypes were produced using multiple design specifications to identify ideal vehicle performance. Multiple metrics, such as vehicle length, vehicle weight, spoiler angle, drivetrain, and ground clearance, were collected for each vehicle. R was used to design a linear model that predicts the mpg of MechaCar prototypes using several variables from the MechaCar_mpg.csv file. 

[OUTPUT FROM LINEAR REGRESSION]

Interpretation of the multiple linear regression results

Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
Vehicle ground clearance, and vehicle length provided non-random amounts of variance to the model.  Both had a significant impact on MPG.


Is the slope of the linear model considered to be zero? Why or why not?
The slope of this linear model is not considered to be zero as the P-value is 5.35e-11

Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
Based on an r-squared value of 0.7149, 71% of mpg predictions can be made using this model.  As a result this model has the ability to predict the mgp of MechaCar prototypes effective. 

## Summary Statistics on Suspension Coils

The MechaCar Suspension_Coil.csv dataset contains the results from multiple production lots. In this dataset, the weight capacities of multiple suspension coils were tested to determine if the manufacturing process is consistent across production lots. Using R, created a summary statistics table to show:

The suspension coil’s PSI continuous variable across all manufacturing lots
The following PSI metrics for each lot: mean, median, variance, and standard deviation.

[Total Summary]
[Lot Summary]

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. With a variance of 62.29 PSI across the manufacuring lots this meets this design specification.  Individually Lot 1 and Lot 2 are within the acceptable PSI design specification with variances of 0.9795918 and 7.4693878 respectively.  Lot 3, however, does individually exceed the design specification pertaining to the variance of suspension coils with a variance of 170.2861224.

## T-Tests on Suspension Coils

T-tests were performed to determine if all manufacturing lots and each lot individually are statistically different from the population mean of 1,500 pounds per square inch.

[t-tests across all Lots]

The mean across all manufacturing lots is 1497.507 at the 95% confidence level and overall mean is 1498.78,  which is similar to the population mean of 1,500 pounds per square inch.

[t-tests across individual Lots]

Lot 1
Mean 95 percent confidence interval:  1499.719
Mean:  1500 

Lot 2
Mean 95 percent confidence interval:  1499.423 
Mean:  1500.2 

Lot 3
Mean 95 percent confidence interval:  1492.431
Mean:  1496.14 

Individually all lots are also similar to the population mean of 1,500 pounds per square inch.