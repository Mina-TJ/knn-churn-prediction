# Customer Churn Prediction using kNN

## What is this project about?
This project predicts which telecom customers are likely to cancel their service (churn).
By identifying at-risk customers early, the company can reach out with special offers to keep them.

## Dataset
- **Source:** Telco Customer Churn dataset
- **Size:** ~7,000 customers
- **Key features:** contract type, monthly charges, tenure, internet service, payment method

## What I did
- Explored why **accuracy is misleading** for imbalanced data (~73% non-churners, ~27% churners)
- Built a **kNN classifier** and evaluated it using **ROC/AUC** instead of accuracy
- Used **bootstrap validation** to tune the best value of k (found k = 102)
- Found the **optimal decision threshold** using Youden's J statistic (threshold = 0.23)

## Key Results
| Metric | Value |
|--------|-------|
| Test AUC | 0.833 |
| Optimal k | 102 |
| Optimal Threshold | 0.23 |
| Sensitivity at optimal threshold | 85% |

## Tools & Libraries
- **Language:** R
- **Libraries:** caret, ROCR, pROC, tidyverse, kableExtra

## Course
MBAN 5560 - Master of Business Analytics, Saint Mary's University

## Live Report
👉 [Click here to view the full analysis](https://mina-tj.github.io/knn-churn-prediction/A3_student.html)
