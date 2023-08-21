# Matplotlib-Challenge: Pymaceuticals SCC Study Analysis
Welcome to the Matplotlib Challenge, a class assignment for my Data Analytics BootCamp at Washignton University. In this project, I will analyze the results of an animal study by Pymaceuticals. The study is focused on potential treatments for squamous cell carcinoma (SCC), a common type of skin cancer. The task is to perform a comprehensive analysis of the study's data and generate essential tables and figures for the technical report. This project will showcase data analytics skills and ability to derive meaningful insights from complex data.

### Background
The Pymaceuticals, Inc., a new pharmaceutical company that specializes in anti-cancer medications; recently began screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer.
In this study, 249 mice who were identified with SCC tumors received treatment with a range of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals’ drug of interest, Capomulin, against the other treatment regimens.

The executive team needs all of the tables and figures for the technical report of the clinical study and a top-level summary of the study results. 

### Tasks
1. Prepare the Data
Import required packages and data files.
Merge mouse_metadata and study_results DataFrames into one.
Identify unique mice IDs and check for duplicate time points.
Remove data associated with any mouse ID having duplicate time points.

2. Generate Summary Statistics
Create a DataFrame containing summary statistics for each drug regimen.
Include statistics such as mean, median, variance, standard deviation, and SEM of tumor volume.

3. Create Bar and Pie Charts
Generate two sets of bar charts displaying the total number of rows (Mouse ID/Timepoints) for each drug regimen throughout the study.
Produce two pie charts illustrating the distribution of female and male mice in the study.

![image](https://github.com/agorvie/Matplotlib-Challenge/assets/122469792/6cdcc6eb-7a01-437b-9b2a-7e3d11407b4e)

![image](https://github.com/agorvie/Matplotlib-Challenge/assets/122469792/66fb1625-b177-4d3b-a5bf-adb397d884d8)

4. Calculate Quartiles, Find Outliers, and Create Box Plot
Calculate final tumor volumes for selected treatment regimens (Capomulin, Ramicane, Infubinol, and Ceftamin).
Compute quartiles, IQR, and identify potential outliers.
Generate a box plot showcasing the distribution of final tumor volumes for each treatment group, highlighting outliers.

![image](https://github.com/agorvie/Matplotlib-Challenge/assets/122469792/edbfb685-af29-45a7-8506-21ae1553c3bc)

5. Create Line Plot and Scatter Plot
Create a line plot demonstrating tumor volume vs. time point for a single mouse treated with Capomulin.
Generate a scatter plot depicting the relationship between mouse weight and average observed tumor volume for the Capomulin regimen.

![image](https://github.com/agorvie/Matplotlib-Challenge/assets/122469792/a45ac0c7-033c-4789-80c0-a34ceda2191f)

![image](https://github.com/agorvie/Matplotlib-Challenge/assets/122469792/22533049-5cf6-4c5a-9bca-de93566ea3d0)

6. Calculate Correlation and Regression
Calculate the correlation coefficient between mouse weight and average tumor volume.
Perform linear regression analysis to model the relationship between mouse weight and tumor volume.
Plot the linear regression model over the scatter plot.

![image](https://github.com/agorvie/Matplotlib-Challenge/assets/122469792/a4d70d3b-67dc-4f29-8628-2bf45666f367)

Correlation coefficient: 0.84

Slope: 0.95

Intercept: 21.55

R-value: 0.84

P-value: 0.00

Standard error: 0.13

## Analysis Summary:
Given that correlation coefficient measures the strength and direction of the linear relationship between two variables,the correlation coefficient value of 0.84 indicates a strong positive correlation between mouse weight and average tumor volume for the Capomulin regimen. This means that as mouse weight increases, the average tumor volume tends to increase as well.

The slope of the linear regression line represents the change in the average tumor volume for each unit increase in mouse weight. In this case, the positive slope of the linear regression line (calculated as 0.95) indicates that for every 1 gram increase in mouse weight, the average tumor volume increases by 0.95 mm3.

The intercept of the linear regression line (calculated as 21.55) represents the estimated average tumor volume when mouse weight is 0 grams. However, since it is not possible to have a mouse with 0 grams weight, the intercept may not have a meaningful interpretation in this context.

The p-value (calculated as 0.00) is a measure of the statistical significance of the linear regression model. In this case, a p-value of 0.00 indicates that the linear regression model is highly statistically significant, suggesting that there is a significant linear relationship between mouse weight and average tumor volume for the Capomulin regimen.

A lower standard error indicates a more precise estimate of the slope. In this case, a standard error of 0.13 suggests a relatively low variability and a relatively precise estimate of the slope in the Capomulin regimen.

However, it’s important to note that correlation does not imply causation, and other factors may also be influencing the relationship between mouse weight and tumor volume. Further analysis and experimentation would be needed to establish causality and make definitive conclusions.

