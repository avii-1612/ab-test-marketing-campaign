# A/B Test Analysis: Marketing Campaign

## Overview
Analysis of an A/B test to find out whether an advertisement increases customer conversion compared to a control group (public service announcement).

**Tools:** Python, pandas, SciPy, NumPy

## Dataset
Marketing A/B Testing dataset from Kaggle (588,101 users).
- **ad group:** 564,577 users
- **psa group (control):** 23,524 users

## Method
1. Calculated the conversion rate of each group
2. Computed absolute and relative lift
3. Ran a two-proportion z-test (H0: both groups have the same conversion rate)
4. Calculated a 95% confidence interval for the difference

## Results
| Metric | Value |
|---|---|
| Ad conversion rate | 2.55% |
| Control conversion rate | 1.79% |
| Absolute lift | +0.77 percentage points |
| Relative lift | +43% |
| z-statistic | 7.37 |
| p-value | < 0.001 |
| 95% CI (difference) | [0.60, 0.94] percentage points |

## Recommendation
**Launch.** The lift is statistically significant and the whole confidence interval is above zero.

## Files
- `ab_test_analysis.ipynb`: full analysis notebook
