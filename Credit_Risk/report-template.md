# Module 20 Report

## Overview

The purpose of this analysis was to determine whether or not a borrower is at a high-risk for defaulting on a potential loan. The dataset used to train the model included prior loan-risk evaluations containing information on the size of the loan, the interest rate charged, the borrower's annual income, total debt, and debt-to-income ratio, as well as the number of accounts the borrower has, as well as any derogatory marks.

A supervised learning model using logistic regression was used to create predictions as to whether potential borrowers were at high-risk for default.

## Results

              precision    recall  f1-score   support

     Healthy       1.00      1.00      1.00     18759
       Risky       0.87      0.89      0.88       625

    accuracy                           0.99     19384
   macro avg       0.94      0.94      0.94     19384
weighted avg       0.99      0.99      0.99     19384

## Summary

Ultimately the model was proficient at predicting whether a loan was low-risk, with a 100% precision and 100% recall, while only having 87% precision and 89% recall at identifying high-risk borrowers. This is likely due to the imbalance of the data set, with 75036 of the 77536 samples (96.78%) being considered low-risk, while only 2500 of the 77536 samples (3.22%) were considered high-risk.
It seems more valuable to be able to predict when a borrower is at a high risk to default than if they are at a low risk, and thus I would be suspect to use this model to determine credit-worthiness.
