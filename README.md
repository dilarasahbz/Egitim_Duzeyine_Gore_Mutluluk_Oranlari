# Happiness by Education Level: An Applied Statistical Analysis

An applied statistics project analyzing the relationship between educational attainment and reported happiness rates in Turkey using official Turkish Statistical Institute (TurkStat / TÜİK) data (2004–2022). The study incorporates exploratory data analysis, parametric and non-parametric hypothesis testing, and linear regression modeling.

---

## 📌 Project Overview
* **Domain:** Applied Statistics, Socioeconomic Data Analysis
* **Tools & Environment:** R, Quarto (`.qmd`), RStudio
* **Team Size:** 5 Contributors

---

## 📊 Dataset
The analysis uses longitudinal survey data from **TurkStat's Household Life Satisfaction Surveys (2004–2022)**, tracking happiness proportions across five educational attainment tiers:
* Higher Education (Bachelor's / Postgraduate)
* High School & Vocational Equivalents
* Primary or Lower Secondary School
* Primary School
* No Formal Education

---

## 🔬 Methodology & Pipeline

1. **Data Ingestion & Inspection:** Structural checks, parsing, and tabular formatting (`readxl`, `str()`, `flextable`).
2. **Exploratory Data Analysis (EDA):** Central tendency, spread, and quantiles (mean, median, standard deviation, IQR).
3. **Data Visualization:** Univariate and bivariate distributions using `ggplot2` (histograms, box plots, scatter plots, grouped bar charts, and dual-axis line charts).
4. **Hypothesis Testing:**
   * One-sample and two-sample proportion tests
   * Independent sample t-tests comparing historical benchmarks (2004 vs. 2022)
5. **Categorical Association:** Chi-Square ($\chi^2$) tests of independence evaluating dependencies between education level, time (year), and happiness levels.
6. **Variance Analysis:** F-tests for equality of variances across demographic groupings.
7. **Regression Modeling:** Ordinary Least Squares (OLS) regression to evaluate the magnitude and significance of education levels on happiness rates.

---

## 📦 Tech Stack & Dependencies

```r
install.packages(c(
  "readxl", "tidyverse", "knitr", "kableExtra", 
  "flextable", "ggplot2", "dplyr", "car", "ggpubr"
))
