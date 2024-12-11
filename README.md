# Bank Marketing Campaign Analysis and Predictive Modeling

## Project Summary

### Project Objective
The objective of this project was to analyze bank marketing campaign data and build a predictive model to classify whether a customer will subscribe to a term deposit (represented by the target variable `y`: 1 for "yes" and 0 for "no"). The project evaluated individual machine learning models and combined them using a stacking ensemble approach to achieve higher predictive accuracy.

---

### Dataset Overview
The dataset contains demographic, campaign, and economic attributes of bank customers, including columns such as:
- **Age, Job, Marital, Education, Default:** Demographic information.
- **Housing, Loan, Contact, Month, Day of Week:** Financial and campaign-related details.
- **Duration, Campaign, Pdays, Previous, Poutcome:** Campaign performance metrics.
- **Emp Var Rate, Cons Price Idx, Cons Conf Idx, Euribor3m, Nr Employed:** Economic indicators.
- **y:** Target variable indicating whether the customer will subscribe to a term deposit.

---

### Models Evaluated
#### 1. **K-Nearest Neighbors (KNN)**
- **Accuracy:** 93%
- **Strengths:** High recall for classifying positive responses.

#### 2. **Support Vector Machine (SVM)**
- **Accuracy:** 94%
- **Strengths:** Balanced precision and recall for both classes.

#### 3. **Decision Tree**
- **Accuracy:** 82%
- **Strengths:** Simple and interpretable.

#### 4. **Naive Bayes**
- **Accuracy:** 84%
- **Strengths:** Handles categorical data effectively.

#### 5. **Stacking Ensemble**
- **Accuracy:** 95%
- **Strengths:** Combines strengths of all models, achieving the highest accuracy.

---

### Key Findings
- **Stacking Model:** Achieved the highest accuracy (95%), demonstrating the effectiveness of combining multiple models.
- **Feature Importance:** Duration and economic indicators (e.g., `euribor3m`, `nr_employed`) significantly influenced predictions.
- **Outcome Prediction:** The `y` prediction indicates whether a customer will get the term deposit based on their demographic, campaign, and economic attributes.
- **Challenges:** Handling missing values in the dataset and optimizing hyperparameters.

---

### Conclusion
The stacking ensemble outperformed individual models in predicting customer responses to the marketing campaign. This approach can be effectively applied to similar classification problems in banking or other domains to predict whether a user will subscribe to a service or product.
