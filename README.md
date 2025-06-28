#Personal Loan Campaign Prediction – Machine Learning Project

##Problem Statement

This project aims to predict whether a liability customer will accept a personal loan offer using historical data. The goal is to:

- Predict loan acceptance using customer attributes.
- Identify key features that influence loan acceptance.
- Recommend which customer segments to target for future campaigns.

---

##Data Dictionary

| Column Name         | Description |
|---------------------|-------------|
| `ID`                | Customer ID |
| `Age`               | Age in completed years |
| `Experience`        | Professional experience (years) |
| `Income`            | Annual income (in $1000s) |
| `ZIP Code`          | ZIP Code of residence |
| `Family`            | Family size |
| `CCAvg`             | Monthly credit card spend (in $1000s) |
| `Education`         | Education level (1: Undergrad, 2: Graduate, 3: Advanced/Professional) |
| `Mortgage`          | Home mortgage value (in $1000s) |
| `Personal_Loan`     | Target variable: 1 if accepted, 0 otherwise |
| `Securities_Account`| Whether the customer has a securities account |
| `CD_Account`        | Whether the customer has a CD account |
| `Online`            | Uses internet banking |
| `CreditCard`        | Owns a credit card from other banks |

---

##Libraries

- Python
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn
- Decision Tree Classifier
- Colab / Jupyter Notebook

---

##Model & Results

- Trained multiple models for binary classification.
- The Decision Tree model with post-pruning** yielded the best performance.
- Evaluation metrics: Accuracy, Recall, Precision, F1-Score

---

##Key Insights

- **High Income** → more likely to accept loans.
- **Larger Family size** → positively correlated with loan acceptance.
- **Education Level 2 & 3** → more likely to opt for loans than Level 1.
- **Higher CCAvg** → more likely to accept loans.
- **Online users are underrepresented** → opportunity to improve digital campaigns.

---

##Business Recommendations

- **Target Segment Focus**: Customers with higher income, larger families, and higher credit card spends.
- **Personalized Campaigns**: Focus efforts on customers with Education Level 2 & 3.
- **Leverage Existing Relationships**: Offer exclusive loan deals to customers with Securities or CD accounts.
- **Improve Digital Engagement**: Launch marketing to increase internet banking usage.
- **Simplify Loan Process**: Streamline the customer journey for faster loan processing and better adoption.

---

##Files Included

- `loan_campaign.html` – Exported HTML version of the notebook
- `README.md` – Project overview and summary
-  Dataset - csv file is present
---

##Future Scope

- Implement more advanced models like Random Forest or XGBoost.
- Incorporate cross-validation and hyperparameter tuning.
- Visualize customer segments with clustering (e.g., K-Means).
- Build a Streamlit app for real-time predictions.

