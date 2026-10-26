# PR. 2 Derivable Judgement: A Statistical Decision-Making Model

## Project Overview
Derivable Judgement is a Python-based statistical analysis project that explores relationships between health indicators using statistical tests, confidence intervals, covariance, correlation, and data visualizations.

## Objectives
- Analyze health data using descriptive statistics.
- Calculate 95% confidence intervals.
- Compare glucose levels between diabetes and non-diabetes groups.
- Test the association between smoking status and diabetes.
- Examine diabetes rates across age groups.
- Calculate covariance and correlation between age and BMI.
- Visualize health data using charts.

## Dataset
**File:** `Derivable_Judgement.csv`

The dataset includes:
- Age and age group
- Weight and BMI
- Blood pressure
- Gender and region
- Smoking status and exercise frequency
- Diabetes and hypertension
- Cholesterol and glucose levels
- Visit date
- Record ID

## Technologies Used
- Python
- Pandas
- SciPy
- Matplotlib
- Seaborn
- Statsmodels

## Statistical Analysis

### 1. Z-test: Glucose Levels vs. Diabetes
- Z-statistic: 17.766
- P-value: 1.2888 × 10⁻⁷⁰

**Conclusion:** Reject H₀. Mean glucose levels differ significantly between the diabetes and non-diabetes groups.

### 2. Chi-square Test: Smoking Status vs. Diabetes
- Chi-square statistic: 12.001
- Degrees of freedom: 2
- P-value: 0.0025

**Conclusion:** Reject H₀. Smoking status and diabetes are significantly associated in the dataset.

### 3. ANOVA: Diabetes Indicator Across Age Groups
- F-statistic: 49.9794
- P-value: 2.9561 × 10⁻²⁶

**Conclusion:** The analysis found a significant difference across age groups. However, a chi-square test is generally more appropriate for comparing rates of a binary disease outcome.

### 4. Covariance and Correlation: Age vs. BMI
- Covariance: 35.7781
- Correlation: 0.5478

**Conclusion:** Age and BMI show a moderate positive linear relationship in the dataset.

### 5. Confidence Intervals
95% confidence intervals were calculated for numerical variables, including age, weight, BMI, blood pressure, cholesterol, and glucose.

## Visualizations
The project creates charts such as:

- `fig1_diabetes_by_smoking.png` — Diabetes prevalence by smoking status
- `fig3_glucose_dist.png` — Glucose level distribution
- `fig4_bp_by_age.png` — Blood pressure by age group
- `fig5_bmi_bp_scatter.png` — BMI versus blood pressure
- `fig6_corr_matrix.png` — Correlation matrix

Charts are saved in the `charts/` folder.

## How to Run the Project
1. Clone or download this repository.
2. Ensure the CSV dataset is in the same folder as the notebook.
3. Install the required libraries:

   ```bash
   pip install pandas scipy matplotlib seaborn statsmodels
   ```

4. Open `Derivable_Judgement.ipynb` in Jupyter Notebook or JupyterLab.
5. Run the notebook cells in order.

## Hypothesis Testing Decision Rule
Using a significance level of 0.05:

- If p-value < 0.05, reject H₀.
- If p-value ≥ 0.05, fail to reject H₀.

## Limitations
- Statistical association does not prove causation.
- Results depend on the quality and size of the dataset.
- Verify reported statistics against the current dataset before submission.
- A chi-square test is generally preferable for comparing disease rates across categorical age groups.

## Repository Contents
- `Derivable_Judgement.csv` — Dataset
- `Derivable_Judgement.ipynb` — Python analysis notebook
- `Theory Notes.docx` — Supporting theory notes
- `requirements.txt` — Dependencies
- `Images/` — Image assets
- `README.md` — Project documentation

## Author
**Tushar Bagle**
