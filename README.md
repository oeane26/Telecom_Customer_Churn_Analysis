# Telecom_Customer_Churn_Analysis
Telecommunication Customer Churn Analysis & Prediction of Orange Côte d’Ivoire

Executive Summary

Telecommunications companies risk losing recurring revenue when customers leave. Because retention resources are limited, identifying high-risk customers and contract segments is essential.

This project analyzes 7,500 customer records to quantify churn, assess potential revenue exposure, and evaluate whether machine learning can support targeted retention efforts.

The analysis identified 889 churned customers, representing an overall churn rate of 11.85% and an estimated $430,138 in revenue at risk. Monthly-contract customers had a higher churn rate than 24-month-contract customers: 13.42% versus 8.96%. This difference suggests that contract structure may influence retention.

The models produced different performance trade-offs. Random Forest achieved higher overall accuracy at 83%, while Logistic Regression identified more churned customers, with recall of 58% compared with 20% for Random Forest. Because missed churners may represent lost revenue, recall and F1 score are more relevant than accuracy alone for this business problem.

Recommended actions include prioritizing retention analysis for monthly-contract customers, investigating regions with substantial revenue exposure, and testing proactive outreach for customers with repeated complaints or service incidents. Before deployment, the models should be validated on operational data, calibrated to business costs, and improved through feature engineering and threshold tuning.

Tools & Technologies

* Python (Pandas, Scikit-learn, Matplotlib)
* SQL
* Tableau
* Google Colab
* GitHub

Business Questions

* What percentage of customers are leaving?
* Which regions and contract types have higher churn rates?
* How much revenue is potentially at risk?
* Can machine learning help identify customers likely to churn?

Key Findings

* Total customers: 7,500
* Churned customers: 889
* Overall churn rate: 11.85%
* Estimated revenue at risk: $430,138
* Monthly-contract churn rate: 13.42%
* 24-month-contract churn rate: 8.96%

Machine Learning

Two classification algorithms were evaluated using an 80/20 stratified train-test split.

Metric	Logistic Regression	Random Forest
Accuracy	64%	83%
Churn Recall	58%	20%
Churn F1	0.28	0.21
ROC-AUC	0.6644	0.6369

Interpretation: Logistic Regression identified more churned customers, while Random Forest achieved higher overall accuracy. Because churn was relatively uncommon, accuracy alone was not sufficient to assess model usefulness. Recall and F1 score provided more relevant measures for identifying potential churners.

Model Comparison

Business Recommendations

* Investigate retention opportunities among monthly-contract customers.
* Prioritize regions with substantial revenue exposure.
* Test proactive outreach for customers with repeated complaints or service incidents.
* Validate model performance on operational data before deployment.

Future Improvements

* Improve classification performance through feature engineering and threshold tuning.
* Add model interpretability analysis.
* Publish the interactive Tableau dashboard.
