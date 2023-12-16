# PHP2550_project2

This is the Project 2: Regression Analysis for PHP2550 Practical Data Analysis class at Brown School of Public Health. The code performs exploratory data analysis for the study population and missing data, as well as model selection processes with methods of LASSO, Best Subset, and Forward selection. All three methods are combined with multiple imputation and cross validation to increase robustness.



In the study population EDA, it was examined the population summary by outcome and center respectively. The model selection processes are decided to be LASSO, Best Subset, and Forward selection. Another common model Ridge is excluded, as it does not perform variable selection. The three models all include variable selection before computing the final model coefficients by regularization. 



The code files contains sections in order of a scientific research paper.

*  1 Introduction
* 2 Study population
  * summary tables with `tbl_summary`
* 3 Method
  * multiple imputation and test split with `mice`
  * cross-validated model selections (each with a written function to help reproducibility)
    * LASSO using package `glmnet`
    * Best Subset using package `L0Learn`
  * model evaluation metrics and plots
    * discrimination and calibration
* 4 Results 
  * correlation
  * missingness
  * model coefficients and occurrence count of exclusion
  * model evaluation
* 5 Discussion
  * test including or excluding `center` and evaluated 
* 6 Conclusion
* 7 Code appendix 



**Additional Libraries Used**

`dplyr`, `tidyverse` - for data manipulation

`ggmice` - for missing data visualization

`gtsummary` - for summary table

`KableExtra` - for neat kable output

`pROC` - for model evaluations

`corrplot` for correlation plot