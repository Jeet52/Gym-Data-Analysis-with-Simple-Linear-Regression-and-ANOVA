# Gym Data Analysis (STAT 382 – Project 2)

**Author:** Jeet Patel  
**Date:** March 2025

---

## Project Overview

This project analyzes a dataset of gym members to understand how workout habits and physical characteristics influence calories burned and water intake. Using statistical methods learned in STAT 382, including regression and ANOVA, the analysis provides insights that can help personalize fitness and hydration plans.

---

## Tools & Methods

- **Programming Language:** R  
- **Reporting:** R Markdown (with knitted HTML and PDF outputs)  
- **Statistical Techniques:**  
  - Simple and multiple linear regression  
  - One-way and two-way ANOVA (with interaction terms)  
  - Diagnostic checks for model assumptions  
- **Data Visualization:** Scatterplots, bar charts, Q-Q plots, residual plots  

---


## Key Findings

- **Workout frequency** positively and significantly predicts calories burned.  
- **Age, fat percentage, and weight** are significant predictors of water intake.  
- Water intake differs significantly across **BMI classes**, as shown by ANOVA and Tukey’s post-hoc test.  
- The interaction between **workout type and experience level** significantly affects calories burned, highlighting the importance of tailored workout programs.

---

## How to Use This Repository

1. **Clone the repo:**

   ```bash
   git clone https://github.com/yourusername/stat382-project2-gym-analysis.git
Open and run the analysis:
Open report/Gym_Data_Analysis.Rmd in RStudio.
Ensure the dataset gym2.csv is in the data/ folder.
Knit the R Markdown file to generate the HTML or PDF report.
Review the report:
View the HTML file Gym_Data_Analysis.html in your browser for interactive results.
Alternatively, open the PDF version (converted from HTML) for submission or printing.
Dependencies

Ensure these R packages are installed:

install.packages(c("knitr", "car", "lmtest", "ggplot2"))
Contact

For questions or collaborations, please contact Jeet Patel at JeetPatel.CompSci@gmail.com.
