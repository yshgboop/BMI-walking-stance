# BMI and Knee Angle Correlation Project

**Consulting ID:** SAR-RS-25-04-01-CC-40

**Date:** 2025-05-02

**Name of the client:** Chiwhan Choi

**Department:** Sargent College of Health & Rehabilitation Sciences

**Project Summary:**

Obesity significantly impacts musculoskeletal health and alters walking biomechanics. This study aimed to quantify the influence of obesity on knee angle changes during various walking tasks and identify associated anthropometric predictors. We analyzed motion sensor data from 35 participants (12 normal-weight, 23 obese) performing six distinct walking tasks (e.g., preferred speed, obstacle negotiation). Knee angle difference (InitialPeak) was the primary outcome. Exploratory data analysis (EDA), including correlation analysis and Variance Inflation Factor (VIF) assessment, guided variable selection. Linear Mixed-Effects Models (LMM), Generalized Additive Mixed Models (GAMM), and Bayesian Mixed Models were developed, incorporating fixed effects for group, demographics, and selected body measurements, with random intercepts for participant and task. Model performance was compared using ANOVA and 5-fold cross-validation (RMSE, R²). Two-sample t-tests compared knee angle differences between groups for each task. EDA and t-tests revealed significantly reduced knee angle differences in the obese group across most tasks (p < 0.05), suggesting less knee flexion. The final LMM demonstrated the best fit and predictive performance (Avg CV RMSE ≈ 2.59, Avg CV R² ≈ 0.68), identifying significant associations between knee angle difference and Shoulder Breadth (positive), Chest Breadth (negative), Lower Thigh Circumference (negative), Shank Circumference (negative), and A Body Shape Index (ABSI, negative). Significant variability was attributed to both participant and task random effects. In conclusion, obesity is associated with reduced knee flexion during walking, and specific body dimensions beyond BMI contribute significantly to these biomechanical alterations.

**Description of the files in the repository:**

* **`Data Graph .Rmd`**: This R Markdown file appears to contain code for generating data visualizations, specifically comparison graphs (e.g., "Comparison of BN_FF and OB_FF") using ggplot2 to analyze various datasets (NB_FF.csv, OB_FF.csv, etc.) related to stance phase and degrees of movement.
* **`eda.ipynb`**: This Jupyter Notebook file includes Python code for exploratory data analysis. It contains functions to split participant data from a CSV file ('Normalized time series_NB.csv') into separate CSV files for each participant and then saves them. It also includes a section for plotting time series data from 'NB_FF.csv'.
* **`project_report.Rmd`**: This R Markdown file is the source code for the final project report titled "BMI Walking Stance Project Final Report". It includes an abstract, introduction, data description, EDA, modeling details (including different models like LMM, GAMM, and Bayesian Mixed Models), model interpretation, and conclusions. It uses various R libraries like dplyr, ggplot2, lme4, etc., for analysis and visualization.
* **`project_report.pdf`**: This PDF file is the rendered version of the "project_report.Rmd", presenting the final report on the BMI Walking Stance Project.
