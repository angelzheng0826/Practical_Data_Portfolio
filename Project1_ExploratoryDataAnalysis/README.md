# PHP2550_Project1

This is the project 1: Exploratory Data Analysis for PHP2550 Practical Data Analysis class at Brown School of Public Health. The code performs exploratory data analysis based on a specific research goal: examine the effect of Smoke During Pregnancy (SDP) and Environmental Tobacco Smoke (ETS) on the child's externalizing, self-regulation and substance use problems. 



The analysis plan originally was to create composite independent variable that sums up the binary indicators across timepoints for smoking status. That is, for example, the `prenatal_score` would be the total number of "yes" responses to smoking status at each timepoint. There is 3 timepoints, then the range would be 0-3. 



However, this plan did not taking into consideration the timing, and further shrinks the sample size because whenever there is an `NA` response, the sum would be `NA`. Therefore the new analysis plan groups the smoking status in prenatal period/exposure status in postnatal period, and performs EDA with visualization on outcome variables by such group. In this way, the missingness is at each time point level, so the subject with some missing timepoint but all can still be used. 



The code files contain sections: (sub-bullet explaining the content)

* Data Preprocessing
  * Correction of formatting issues and unreasonable entries 

* Demographic Information, univariate
  * Contains tables and histograms that show the demographic information about the data
* Missing Pattern
  * Table of the variables with the most missingness percentage 
  * Missing patterns plots for pre- and post-natal responses 
* Prenatal and Postnatal Smoking, univariate
  * Tables summarizing the responses from prenatal and postnatal period, respectively
* Externalizing Behaviors vs. Prenatal Period Tobacco Exposure
  * how the Independent Variable is constructed and why
  * how the outcome variables "Externalizing" are defined
  * why excluding autism data
  * boxplots for externalizing behaviors by mother's smoking status across timepoints
  * scatterplots and line estimate for externalizing behaviors against mother's cotinine level
* Externalizing Behaviors vs. Postnatal Period Tobacco Exposure
  * boxplots for externalizing behaviors by child's smoke exposure status across timepoints
  * scatterplots and line estimate for externalizing behaviors against child's cotinine level
  * correlation of some possible covariates variables to aid explanation
* Self Emotion Regulation vs. Prenatal Period Tobacco Exposure
  * how the outcome variables "Self-Regulation" are defined
  * boxplots for self-regulation by mother's smoking status across timepoints
  * scatterplots and line estimate for self-regulation against mother's cotinine level
* Self Emotion Regulation vs. Postnatal Period Tobacco Exposure
  * boxplots for self-regulation by child's smoke exposure status across timepoints
  * scatterplots and line estimate for self-regulation against child's cotinine level
  * correlation of some possible covariates variables to aid explanation
* Substance-use vs. Prenatal and Postnatal Period Tobacco Exposure
  * how substance-use is defined and used for plotting
  * barplots for different types of substance-use behaviors, by mother's smoking status across timepoints
* Initial Regression
  * test of whether the effect of variable is statistically significant 
* Conclusion
  * summary of the findings
  * strengths and limitations of the data