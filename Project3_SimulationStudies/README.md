# PHP2550_project3

This is the Project 3: Simulation Studies for PHP2550 Practical Data Analysis class at Brown School of Public Health. The code performs exploratory data analysis for the source and target population, namely Framingham and NHANES 2017, and conducts transportability analysis of a built predictive model for cardiovascular disease. 



The transportability analysis is done in three settings: 

**I Framingham Source Data**

In this section, the source data Framingham is test splitted and model performance is evaluated using sensitivity, specificity, Brier score and AUC. This section only tests the model performance implemented from train source data and tested on test source data. 

**II Composite Data (Framingham + NHANES 2017)**

In this section, the source data Framingham is combined with NHANES 2017, the target population data without outcome variable, to create a composite data. A formula is used to calculate estimate Brier score using the composite data. 

**III Simulation (Framingham + NHANES Simulated)**

In this section, a simulation with iteration = 100 is generated. Each covariate is generated based on its distribution in Framingham data and summary statistics in NHANES data. Then the same formula for Brier score estimator is applied iteratively. Mean of the 100 Brier score estimates yields the final estimate. 