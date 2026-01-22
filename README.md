# Bias Audit of Race in Healthcare Data

## Project Overview

This project performs a bias audit on a clinical dataset (Clinical Data_Discovery_Cohort.csv) to identify and mitigate potential biases in healthcare data. The notebook explores demographic distributions (gender, race, disease stage), evaluates fairness metrics, validates bias patterns using statistical tests, and applies bias mitigation techniques.

## Group Memmbers

- Nthabiseng Mkhehlani
- Rivomba Ndhukwana
- Nqobile Magwaza
- Nkhensani Manganye
- Nqobile Ngwenya

## Objectives

- Analyze distributions of sex, race, and disease stage.
- Investigate how these factors relate to patient outcomes (Dead or Alive).
- Quantify bias using fairness metrics.
- Validate disparities with statistical tests.
- Apply bias mitigation techniques (oversampling).
- Provide a comprehensive summary of findings, implications, and ethical considerations.

## Key Steps

### 1. Data Exploration

- Visualized distributions of gender, race, and disease stage.
- Examined outcome (Dead or Alive) across demographic groups.

### 2. Fairness Metrics

Calculated three fairness metrics for sex and race:

### - Statistical Parity Difference (SPD)
### - Disparate Impact (DI)
### - Equal Opportunity Difference (EOD)

### 3. Statistical Validation

Performed Chi-squared tests for independence:

- sex vs Dead or Alive
- race vs Dead or Alive
- Stage vs Dead or Alive

### 4. Bias Mitigation

- Racial imbalance mitigation: Oversampled underrepresented racial groups (A, O, B).
- Outcome imbalance mitigation: Oversampled the Alive outcome class.
- Visualized distributions after mitigation.

### 5. Comprehensive Summary

- Reviewed identified biases.
- Reported fairness metrics and statistical validation.
- Assessed impact of mitigation strategies.
- Recommended dataset improvements.
- Discussed real-world implications and ethical framework.

## Results & Insights

- Gender Bias: Slight imbalance; males showed higher mortality rates.
- Racial Bias: Severe imbalance; White patients dominated, while Asian and Other groups were underrepresented.
- Stage Bias: Certain disease stages were heavily skewed toward one outcome.
- Fairness Metrics: Indicated disparities across sex and race.
- Chi-squared Tests: Confirmed statistical significance of some disparities.
- Mitigation: Oversampling improved representation and balanced outcomes.

## Ethical Considerations

- Ensure representative sampling across demographics.
- Avoid reinforcing systemic biases in healthcare.
- Apply fairness-aware methods in predictive modeling.
- Recognize potential harms of biased datasets in clinical decision-making.

## How to Run

1. Clone repository and open the notebook.
2. Install dependencies:
```bash

   pip install pandas numpy matplotlib seaborn imbalanced-learn scipy
```



3. Place Clinical Data_Discovery_Cohort.csv in the working directory.
4. Run cells sequentially to reproduce analysis and visualizations.

## Dependencies

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- imbalanced-learn
- scipy

## Future Work

- Expand dataset with more diverse samples.
- Apply advanced fairness-aware algorithms.
- Explore intersectional bias (e.g., race × gender).
- Integrate predictive modeling with fairness constraints.
