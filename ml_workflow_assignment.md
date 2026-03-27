# ML Workflow Assignment

## Task 1: Label and Data Leakage
- **Label (Target Variable):** `repeat_purchase_flag`  
  This column represents the outcome we want to predict — whether a customer makes a repeat purchase within 30 days.  

- **Leaky Feature:** `discount_used_on_repeat_order`  
  This feature is only known after the repeat purchase occurs, so including it would leak future information into the model and make evaluation unreliable.  

---

## Task 2: Essential Steps Before Training a Complex Model
1. **Data Exploration and Cleaning**  
   Before modeling, the dataset should be audited for missing values, outliers, and inconsistencies. This ensures the model learns from clean, reliable data and avoids bias or errors.  

2. **Establishing a Baseline Model**  
   A simple baseline (e.g., predicting the majority class or using logistic regression) provides a benchmark. It helps measure whether the complex gradient boosting model actually adds value beyond trivial predictions.  

---

## Suggested Complete ML Workflow
1. **Data auditing and cleaning** — check quality, ethics, and privacy.  
2. **Feature engineering** — derive useful features, remove leaky ones.  
3. **Train/validation/test split** — prevent overfitting and ensure generalization.  
4. **Baseline model** — establish a simple benchmark.  
5. **Complex model training** — gradient boosting or other advanced methods.  
6. **Evaluation on held-out test set** — final performance check before deployment.  
7. **Deployment with monitoring** — track drift, fairness, and reliability.  

---

## Submission Guidelines
- Save this file as `ml_workflow_assignment.md`.  
- Push it to your GitHub repository under the folder `assignments/`.  
- Share the repository link as your submission.  