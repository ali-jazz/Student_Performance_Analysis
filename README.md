# Student_Performance_Analysis

##  Project Overview

This project explores the factors associated with student academic performance using exploratory data analysis (EDA), hypothesis testing, and statistical modeling techniques in Python.

The objective of this analysis is to identify which academic, behavioral, and socio-economic variables appear most strongly associated with exam performance while applying rigorous statistical reasoning and model diagnostics.

Rather than focusing on predictive machine learning, this project emphasizes:

* statistical interpretation,
* inferential analysis,
* variable relationships,
* model diagnostics,
* and analytical storytelling.

---

#  Dataset

Dataset source:
https://www.kaggle.com/datasets/arfeenkabir/student-performance-factors

The dataset contains student-level information related to:

* study habits,
* attendance,
* tutoring sessions,
* parental involvement,
* educational resources,
* socio-economic indicators,
* lifestyle factors,
* and academic performance.

The target variable analyzed throughout the project is:

* `Exam_Score`

---

#  Research Questions

This project aims to answer the following questions:

* Does attendance significantly impact exam performance?
* Are highly motivated students associated with stronger academic outcomes?
* Which factors appear most strongly associated with academic success?
* Does parental involvement influence academic performance?
* Which variables remain significant after controlling for other factors?

---

#  Methodology

The analysis followed a structured analytical workflow:

1. Data quality validation
2. Data cleaning and preprocessing
3. Exploratory Data Analysis (EDA)
4. Correlation analysis
5. Hypothesis testing using ANOVA
6. Multiple linear regression
7. Forward and backward stepwise variable selection
8. Multicollinearity diagnostics using VIF

---

#  Technologies & Libraries

## Programming Language

* Python

## Libraries

* Pandas
* NumPy
* Matplotlib
* Seaborn
* SciPy
* Statsmodels

---

#  Data Quality Validation

Several validation checks were performed before analysis:

* Missing value detection
* Duplicate observation checks
* Outlier identification using IQR analysis
* Reasonableness checks on exam scores

A small number of exam scores exceeding 100 were identified. These observations were retained, as they may represent grading bonuses rather than clear data entry errors.

---

#  Exploratory Data Analysis

The exploratory phase included:

* distribution analysis,
* correlation heatmaps,
* scatterplots,
* histograms,
* boxplots,
* and categorical group comparisons.

The analysis suggested that:

* attendance,
* study hours,
* parental involvement,
* and access to educational resources

appeared positively associated with academic performance.

---

#  Statistical Analysis

## ANOVA Testing

ANOVA tests were used to determine whether mean exam scores differed significantly across categorical groups such as:

* motivation level,
* parental involvement,
* family income,
* teacher quality,
* and access to educational resources.

Several socio-economic and behavioral variables were found to be statistically associated with exam performance.

Variables such as gender and school type did not appear statistically significant in this dataset.

---

#  Multiple Linear Regression

Multiple linear regression models were developed to evaluate the combined effect of explanatory variables on exam performance.

Both forward and backward stepwise selection approaches were used to identify the variables contributing most meaningfully to the model.

The final model explained approximately:

R^2 = 0.688

This indicates that the model explains nearly 69% of the variance in exam scores.

Key variables retained in the final model included:

* Attendance
* Hours Studied
* Previous Scores
* Tutoring Sessions
* Motivation Level
* Family Income
* Parental Involvement
* Teacher Quality
* Access to Resources
* Internet Access

---

#  Model Diagnostics

Variance Inflation Factor (VIF) diagnostics were performed to evaluate multicollinearity.

All explanatory variables showed acceptable VIF values, suggesting that severe multicollinearity was not present in the final model.

Although the regression output generated a high condition number warning, additional diagnostic analysis suggested that multicollinearity was not problematic in practice.

---

#  Key Findings

* Attendance showed one of the strongest positive relationships with exam performance.
* Study habits and tutoring sessions were positively associated with academic success.
* Access to educational resources and parental involvement remained significant after controlling for other variables.
* Motivation level continued to show a statistically significant effect in multivariate models.
* Gender and school type did not appear significantly associated with exam performance.
* The final regression model explained approximately 69% of the variance in student exam scores.

---

#  Limitations

* Correlation does not imply causation.
* The dataset may not perfectly represent real-world educational systems.
* Some explanatory variables may capture overlapping socio-economic effects.
* The analysis focused primarily on linear relationships.
* Potential interaction effects between variables were not extensively explored.

---

#  Repository Structure

```text
student-performance-analysis/
│
├── data/
│   └── StudentPerformanceFactors.csv
│
├── notebooks/
│   └── Student_Performance.ipynb
│
├── README.md
│
└── LUCENSE
```

---

# 👤 Author

Ali Jazzar

* Actuarial professional
* Data analytics enthusiast
* Interested in statistical modeling, business analytics, and data-driven decision-making
