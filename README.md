# **Socioeconomic Status and Cancer Survival: A Survival Analysis Using Kaplan–Meier and Cox Regression**

-----------
## 📖 **Overview**

Cancer remains a leading cause of mortality worldwide, with patient survival determined not only by tumor biology and clinical care but also by the social and economic conditions in which individuals live. Socioeconomic status (SES), education, and access to healthcare resources has emerged as a critical determinant of cancer outcomes. Patients from lower SES backgrounds often experience barriers to early detection, delayed diagnosis at advanced stages, and reduced access to high-quality treatment and supportive care, all of which contribute to poorer survival. While the association between SES and cancer mortality is well documented, isolating its independent effect requires careful adjustment for established clinical prognostic factors such as age, cancer stage, and treatment setting. Survival analysis techniques, including Kaplan-Meier estimation and Cox proportional hazards regression, offer robust frameworks for examining time-to-event data while accounting for censoring and confounding.

----------
## 🎯 **Objectives**

The primary objective of this project is to evaluate the association between socioeconomic status and overall survival among cancer patients in the Compaq cohort. Specifically, the analysis aims to:

- Compare survival distributions across socioeconomic groups using Kaplan–Meier survival curves and the log-rank test.
- Estimate the association between socioeconomic status and mortality using Cox proportional hazards regression, first in an unadjusted model and then after adjusting for age group, cancer stage, and hospital type.
- Quantify differences in mortality risk across socioeconomic groups using hazard ratios (HRs) and 95% confidence intervals.
- Assess the proportional hazards assumption using Schoenfeld residual tests to evaluate the validity of the Cox regression model and identify potential violations among the included covariates.

-----------
## 📊 **Data Source**

This analysis uses the Compaq cohort data from the epiDisplay R package. The dataset contains individual-level cancer survival data along with socioeconomic and clinical variables.

Key variables:

- `ses`: Socioeconomic status (Rich, High-middle, Poor-middle, Poor)

- `status`: Event indicator (death)

- `year`: Survival time

- `agegr`: Age group

- `stage`: Cancer stage

- `hospital`: Hospital type

------------
## 🛠️ **Tools and Technology Used**

- R
- RStudio
- Tidyverse
- Survival
- Survminer
- gtsummary
- epiDisplay
- ggsurvfit
- quarto

------------
## ⚙️ **Project Workflow**

- Data preparation
- Exploratory data analysis
- Descriptive analysis
- Kaplan-Meier survival analysis
- Cox proportional hazards regression
- Proportional hazards assumption diagnostics

------------------
## 🏆 **Key Outcomes**

- The Kaplan–Meier analysis and log-rank test demonstrated significant differences in survival across socioeconomic groups, with poor socioeconomic status showing less favorable survival compared with the other groups.
- socioeconomic status was significantly associated with mortality; however, after adjustment for age, cancer stage, and hospital type, the association changed, with poor SES remaining significantly associated with a lower estimated hazard relative to the rich group, while the difference for the middle group was no longer statistically significant.
- Age, cancer stage, and hospital type were also important predictors of survival, with older age and more advanced cancer stages associated with substantially higher mortality hazards, whereas treatment in a private hospital was associated with a lower hazard.
- Diagnostic assessment indicated that the proportional hazards assumption was violated for cancer stage.
- The influence diagnostics did not reveal an obvious pattern of extreme influential observations, although individual observations should still be examined when conducting sensitivity analyses.

----------------
## ✅ **Conclusion**

This study evaluated the association between socioeconomic status and overall survival among 1,064 cancer patients from the Compaq cohort using Kaplan–Meier estimation and Cox proportional hazards regression. The findings highlight the importance of considering socioeconomic and clinical factors together when investigating cancer survival and demonstrate the value of survival analysis for identifying disparities in cancer outcomes.




















