# Auditing and mitigating algorithmic unfairness in credit scoring

**Academic project — AMSE, May 2026**  
**Authors:** Loukmane BOULANKI and Céline ADOUSSINGANDE  
**Supervisor:** Prof. Christophe Hurlin

## Research question

How can gender-related disparities in credit-scoring predictions be detected and mitigated, while considering both predictive performance and statistical uncertainty?

## Data and models

The study uses the German Credit dataset (1,000 observations) and compares:
- Logistic Regression;
- Random Forest;
- LightGBM.

The protected-group indicator is constructed from the available dataset fields; its limitations are discussed in the report.

## Methodology

- Exploratory analysis and feature encoding.
- Predictive evaluation on a stratified train/test split.
- Threshold-based fairness diagnostics, including Disparate Impact.
- Inferential fairness testing following Hurlin et al. (2024).
- Fairness Partial Dependence Plot (FPDP) and variable neutralisation at prediction time.

## Main result

For Random Forest, Disparate Impact is approximately 0.88 and therefore passes the four-fifths threshold, while the inferential statistical-parity test rejects the null at 5% (F = 4.53, p = 0.033). Neutralising the feature *Payment Status of Previous Credit* at modality 2 changes the test result to F = 2.49 (p = 0.114), while test accuracy increases from 0.747 to 0.763 and AUC from 0.750 to 0.754.

## Limitations

The dataset is small and dates from 1994. The protected indicator combines gender with marital-status information, and the mitigation procedure focuses on one feature at a time. These limitations constrain external validity and interpretation.

## Materials

- [Python notebook on Google Colab](https://colab.research.google.com/drive/17nu2eLE56w4oA1UsPMfo8DQKROF4DdMr?usp=sharing)
- The full written report should be placed in this folder when its public version is ready.

