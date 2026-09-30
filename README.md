# Happiness by Education Level

A statistics project prepared for the Applied Statistics course using data from TÜİK. The project examines the relationship between education level and happiness rate through descriptive statistics, charts, hypothesis tests, chi-square tests, F distribution, and regression analysis.

**Team:** 5 members

## Data Used

The dataset is the "Happiness Rates by Education Level" data from TÜİK's household surveys. It covers the years 2004-2022 and the following education levels: higher education, high school or equivalent, primary or secondary school, and primary school and did not complete any school.

## Analysis Steps

1. Reading and examining the data (`readxl`, `str()`, `flextable()`)
2. Descriptive statistics (mean, median, standard deviation, quantile)
3. Charts (scatter, histogram, box, bar, pie, bar-line)
4. Hypothesis tests (t-test, one and two population proportion tests)
5. Chi-square tests (independence tests)
6. F distribution and variance test
7. Regression analysis

## Required R Packages

```
readxl, tidyverse, knitr, kableExtra, flextable, ggplot2, dplyr, car, ggpubr
```

## Conclusion

In the t-test, no significant difference was found in the mean happiness of higher education graduates between 2004 and 2022. However, the chi-square independence tests identified statistically significant relationships between happiness and both education level and year. The regression model showed that education level has an overall significant effect on happiness, and that this effect is particularly pronounced at the higher education and primary school levels.
