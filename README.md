# Healthcare Claims Cost Drivers & Risk Analysis

## Overview
This project analyzes healthcare insurance claims data to identify statistically significant drivers of medical costs.  
The objective is to understand which demographic and lifestyle factors are most strongly associated with higher healthcare charges and to translate these findings into business-relevant insights.

The analysis emphasizes interpretability and decision support rather than predictive accuracy.

---

## Problem Statement
Healthcare costs vary significantly across individuals, making it important for insurers and healthcare organizations to understand key cost drivers.  
This project seeks to answer:
- Which factors are most strongly associated with higher medical charges?
- How do these factors behave independently and in combination?
- What insights can support cost management and risk prioritization?

---

## Dataset
The dataset contains anonymized individual-level information, including:
- Age
- Sex
- Body Mass Index (BMI)
- Number of dependents
- Smoking status
- Region
- Annual medical charges billed to insurance

The data is observational and represents aggregated annual costs.

---

## Approach
The analysis follows a structured, statistically grounded workflow:

1. **Exploratory Data Analysis**
   - Distribution analysis of medical charges
   - Identification of skewness and variability patterns

2. **Hypothesis Testing**
   - Two-sample Welch’s t-test to assess cost differences between smokers and non-smokers

3. **Univariate Analysis**
   - Correlation and regression analysis for continuous variables such as BMI and age

4. **Multivariate Regression**
   - Linear regression incorporating age, BMI, and smoking status to isolate independent effects

The focus is on interpretability, effect size estimation, and analytical rigor.

---

## Key Findings
- Smoking status is the strongest independent driver of healthcare costs, associated with a large step-change in expected annual charges.
- Age contributes steady, incremental increases in medical costs.
- BMI shows a statistically significant but smaller incremental effect.
- A multivariate regression model explains approximately **75% of the total variation** in medical charges.

---

## Limitations
- The dataset is observational; results indicate association, not causation.
- Clinical variables such as diagnoses and treatment details are not available.
- Costs are aggregated annually, masking short-term variability.
- Linear relationships are assumed for interpretability.

---

## Next Steps
- Incorporate interaction effects (e.g., age × smoking) to capture subgroup-specific behavior.
- Perform risk segmentation to identify high-cost cohorts.
- Extend analysis using longitudinal or clinical data to support causal insights.

---

## Tools & Libraries
- Python
- Pandas, NumPy
- SciPy, Statsmodels
- Matplotlib, Seaborn

---

## How to Run
1. Install dependencies:
   ```bash
   pip install -r requirements.txt
