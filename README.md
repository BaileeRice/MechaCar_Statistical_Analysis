# MechaCar_Statistical_Analysis

TASKS:

Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes

Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots

Run t-tests to determine if the manufacturing lots are statistically different from the mean population

Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.

---

## Linear Regression to Predict MPG

![image](https://user-images.githubusercontent.com/105184244/193732826-378a9f3a-6d1c-4f6b-8f0c-1127dc09471a.png)

1. Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

The length of the vehicle and its ground clearance provide a non-random amount of variance to the mpg values based off their p-values.
- ground clearance: 0 < .05
- vehicle length: 0 < .05

2. Is the slope of the linear model considered to be zero?

![image](https://user-images.githubusercontent.com/105184244/193736038-c1051bcb-8038-4c4e-aeb3-09cefaba600c.png)

This model has a very low p-value compared to the typical significance value of .05%, therefore the null hypothesis can be rejected and it confirms a non-zero slope.

3. Does this linear model predict mpg of MechaCar prototypes effectively?

![image](https://user-images.githubusercontent.com/105184244/193737229-2aa6d8e3-14ad-49c7-8e03-a9dce1f32da9.png)


Yes and no, the model has a .7149 or 71% prediction efficiency but there is still alot of breathe room there, I suppose its down to how 'effective' we're talking.

---

## Summary Statistics on Suspension Coils

All lots:

![image](https://user-images.githubusercontent.com/105184244/193743550-c7b5eeb0-0752-4f86-aae8-e07f6e6f3d0a.png)

Individual lots:

![image](https://user-images.githubusercontent.com/105184244/193743249-f469ebb0-0e4e-4203-95d2-492bcd9485aa.png)

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually?

Total manufacturing variance rests well in the 100 PSI range at 62 PSI. However, when you take a look at the individual lots you see 'lot 3' sits at a 170 variance. As a whole the summary stats seemed to show a normal PSI range, individually examining the lots proves that not all of them meet the design specifications.

---

## T-Tests on Suspension Coils

![image](https://user-images.githubusercontent.com/105184244/193746560-df9c9762-2568-425d-ba12-801d08f8c2b2.png)

Based off the p-value, one can assume the all the lots as a whole fall within the normal range.

![image](https://user-images.githubusercontent.com/105184244/193746753-720be544-7448-4eec-b133-296e05625c65.png)

Similarly, lot 1 falls into the same category with a p-value of 1.

![image](https://user-images.githubusercontent.com/105184244/193746823-c96c1478-dc2f-4330-9aa2-cac02d953222.png)

Lot 2 being the same way with little difference in distribution, its p-value being .6 relative to the .5 we're comparing this to.

![image](https://user-images.githubusercontent.com/105184244/193746863-4e84946b-7948-488b-bce4-93989a1e9bf9.png)

Lot 3 has a p-value lower than our .5 set point, one can conclude that this is abnormal but interestingly, the mean still rests in the 95 percent confidence interval.

---
