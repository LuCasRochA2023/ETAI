# Lucas Carvalho da Rocha 20260526  

## Decision Tree:
Train accuracy: 0.679
Test accuracy:  0.669

## Logistic Regression(Better):
Train accuracy: 0.678
Test accuracy:  0.679

## Week 3: decision-tree
Classification report (test set):
              precision    recall  f1-score   support

           0       0.70      0.68      0.69       684
           1       0.63      0.65      0.64       568

    accuracy                           0.67      1252
   macro avg       0.67      0.67      0.67      1252
weighted avg       0.67      0.67      0.67      1252

False positive rate by race
(share of people who did NOT reoffend, but were predicted to)

  Our model:
     African-American    FPR = 0.67  (n=6)
     Caucasian           FPR = 0.00  (n=1)
    -                    FPR = 0.20  (n=5)
    ?                    FPR = 0.33  (n=3)
    AFRICAN-AMERICAN     FPR = 0.00  (n=4)
    African American     FPR = 0.33  (n=3)
    African-American     FPR = 0.39  (n=303)
    Asian                FPR = 0.33  (n=3)
    CAUCASIAN            FPR = 0.25  (n=4)
    Caucasian            FPR = 0.31  (n=232)
    Hispanic             FPR = 0.15  (n=61)
    Native American      FPR = 0.00  (n=2)
    Other                FPR = 0.15  (n=41)
    african-american     FPR = 0.20  (n=10)
    caucasian            FPR = 0.33  (n=3)
    hispanic             FPR = 0.33  (n=3)

  COMPAS's own score:
     African-American    FPR = 0.50  (n=6)
     Caucasian           FPR = 0.00  (n=1)
    -                    FPR = 0.20  (n=5)
    ?                    FPR = 0.00  (n=3)
    AFRICAN-AMERICAN     FPR = 0.25  (n=4)
    African American     FPR = 0.33  (n=3)
    African-American     FPR = 0.44  (n=303)
    Asian                FPR = 0.00  (n=3)
    CAUCASIAN            FPR = 0.25  (n=4)
    Caucasian            FPR = 0.25  (n=232)
    Hispanic             FPR = 0.15  (n=61)
    Native American      FPR = 0.50  (n=2)
    Other                FPR = 0.20  (n=41)
    african-american     FPR = 0.50  (n=10)
    caucasian            FPR = 0.00  (n=3)
    hispanic             FPR = 0.33  (n=3)

## Week 3: Logistic regression

Train accuracy: 0.680
Test accuracy:  0.681
Gap (train - test): -0.000

Classification report (test set):
              precision    recall  f1-score   support

           0       0.69      0.74      0.72       684
           1       0.66      0.60      0.63       568

    accuracy                           0.68      1252
   macro avg       0.68      0.67      0.67      1252
weighted avg       0.68      0.68      0.68      1252

False positive rate by race
(share of people who did NOT reoffend, but were predicted to)

  Our model:
     African-American    FPR = 0.50  (n=6)
     Caucasian           FPR = 0.00  (n=1)
    -                    FPR = 0.20  (n=5)
    ?                    FPR = 0.33  (n=3)
    AFRICAN-AMERICAN     FPR = 0.00  (n=4)
    African American     FPR = 0.33  (n=3)
    African-American     FPR = 0.33  (n=303)
    Asian                FPR = 0.33  (n=3)
    CAUCASIAN            FPR = 0.25  (n=4)
    Caucasian            FPR = 0.23  (n=232)
    Hispanic             FPR = 0.10  (n=61)
    Native American      FPR = 0.00  (n=2)
    Other                FPR = 0.12  (n=41)
    african-american     FPR = 0.10  (n=10)
    caucasian            FPR = 0.00  (n=3)
    hispanic             FPR = 0.33  (n=3)

  COMPAS's own score:
     African-American    FPR = 0.50  (n=6)
     Caucasian           FPR = 0.00  (n=1)
    -                    FPR = 0.20  (n=5)
    ?                    FPR = 0.00  (n=3)
    AFRICAN-AMERICAN     FPR = 0.25  (n=4)
    African American     FPR = 0.33  (n=3)
    African-American     FPR = 0.44  (n=303)
    Asian                FPR = 0.00  (n=3)
    CAUCASIAN            FPR = 0.25  (n=4)
    Caucasian            FPR = 0.25  (n=232)
    Hispanic             FPR = 0.15  (n=61)
    Native American      FPR = 0.50  (n=2)
    Other                FPR = 0.20  (n=41)
    african-american     FPR = 0.50  (n=10)
    caucasian            FPR = 0.00  (n=3)
    hispanic             FPR = 0.33  (n=3)

### Detais week 3

It was worth treating the data to test a new dataset. The result showed that Logistc Regression achieved higher  accuracy, better generalization and less overfitting.