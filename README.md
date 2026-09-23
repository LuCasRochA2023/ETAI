# Lucas Carvalho da Rocha
## 20260526

# COMPAS Recidivism Prediction

This project evaluates and compares predictive models for recidivism risk using the COMPAS dataset. The goal is to predict whether a person will reoffend within two years and to assess fairness across demographic groups.

## Model comparison

### Decision Tree
- Train accuracy: 0.682
- Test accuracy: 0.669
- Gap (train - test): +0.012

### Logistic Regression
- Train accuracy: 0.676
- Test accuracy: 0.657
- Gap (train - test): +0.019

## Week 3: Decision Tree

### Classification report (test set)

| Class | Precision | Recall | F1-score | Support |
|-------|-----------|--------|----------|---------|
| 0 | 0.68 | 0.77 | 0.72 | 793 |
| 1 | 0.66 | 0.55 | 0.60 | 650 |

- Accuracy: 0.67
- Macro avg: 0.67
- Weighted avg: 0.67

### False positive rate by race

Share of people who did not reoffend but were predicted to.

#### Our model
- African-American: FPR = 0.32 (n=349)
- Asian: FPR = 0.00 (n=2)
- Caucasian: FPR = 0.19 (n=290)
- Hispanic: FPR = 0.11 (n=85)
- Native American: FPR = 0.00 (n=1)
- Other: FPR = 0.17 (n=54)

#### COMPAS's own score
- African-American: FPR = 0.44 (n=349)
- Asian: FPR = 0.00 (n=2)
- Caucasian: FPR = 0.24 (n=290)
- Hispanic: FPR = 0.16 (n=85)
- Native American: FPR = 1.00 (n=1)
- Other: FPR = 0.20 (n=54)

> Full results saved to: results/run_20260923_215138.txt

## Week 3: Logistic Regression

### Classification report (test set)

| Class | Precision | Recall | F1-score | Support |
|-------|-----------|--------|----------|---------|
| 0 | 0.65 | 0.80 | 0.72 | 793 |
| 1 | 0.66 | 0.48 | 0.56 | 650 |

- Accuracy: 0.66
- Macro avg: 0.66
- Weighted avg: 0.66

### False positive rate by race

#### Our model
- African-American: FPR = 0.28 (n=349)
- Asian: FPR = 0.00 (n=2)
- Caucasian: FPR = 0.14 (n=290)
- Hispanic: FPR = 0.11 (n=85)
- Native American: FPR = 0.00 (n=1)
- Other: FPR = 0.19 (n=54)

#### COMPAS's own score
- African-American: FPR = 0.44 (n=349)
- Asian: FPR = 0.00 (n=2)
- Caucasian: FPR = 0.24 (n=290)
- Hispanic: FPR = 0.16 (n=85)
- Native American: FPR = 1.00 (n=1)
- Other: FPR = 0.20 (n=54)

### Details week 3

It was worth treating the data to test a new dataset. The result showed that Decision Tree achieved higher accuracy, better Macro avg and Weighted avg.