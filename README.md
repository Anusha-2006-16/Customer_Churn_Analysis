<img width="1393" height="807" alt="Screenshot 2026-04-03 125816" src="https://github.com/user-attachments/assets/e890c6d8-965c-40ac-8e8e-104943d95f0e" /># Customer_Churn_Analysis
Customer churn is a critical problem for subscription-based businesses, as losing customers directly impacts revenue. This project focuses on analyzing customer behavior and building predictive models to identify customers who are likely to churn.


1) EDA Insights

A . Customers on month-to-month contracts are highly likely to churn, indicating lack of long-term commitment
B . New customers (low tenure) are at highest risk → need early engagement
C . Fiber optic users show higher churn, possibly due to pricing or service dissatisfaction
------------------------------------------------------------------------------------------------
2) Feature Engineering

Segmented customers into tenure-based cohorts to capture lifecycle-based churn behavior
--------------------------------------------------------------------------------------------------
3. Model Choice Justification (IMPORTANT)

used:

RandomForestClassifier(class_weight='balanced', n_estimators=250, max_depth=5)
======
Used class_weight='balanced' to handle class imbalance
Limited max_depth=5 to prevent overfitting
Increased n_estimators=250 for better stability
----------------------------------------------------------------------------------------------------
🔝 Most Important Features
1. Tenure (0.149)

👉 Most powerful predictor

Interpretation:

New customers are much more likely to churn
Long-term customers are stable

✅ Business Insight:

Focus on retaining customers in the first few months

2. Contract Type
Two-year contract → very high importance
One-year contract → also significant

Interpretation:

Longer contracts = lower churn
Month-to-month = highest churn risk

✅ Business Insight:

Encourage long-term contracts with discounts or benefits

3. Service Features
Online Security
Tech Support

Interpretation:

Customers without these services churn more

✅ Business Insight:

Bundle security + support services to improve retention

4. Internet Service (Fiber Optic)

👉 High importance

Interpretation:

Fiber optic users are more likely to churn

✅ Possible reasons:

Expensive
Service quality issues

✅ Business Insight:

Re-evaluate pricing or improve service quality

5. Charges (Total + Monthly + Avg)

👉 Strong influence

Interpretation:

Higher spending customers are more sensitive

✅ Business Insight:

Offer personalized pricing or loyalty discounts

6. Payment Method (Electronic Check)

👉 Important churn indicator

Interpretation:

These users churn more

✅ Business Insight:

Promote auto-pay methods for better retention

-------------------------------------------------------------------------------------------------
🎯 Retention Strategy
1.Target New Customers
  	Focus on first 6–12 months
	Provide onboarding offers
2.Promote Long-Term Contracts
	Discounts for yearly plans
	Loyalty programs
3.Improve Service Quality
	Especially for fiber optic users
4.Bundle Value Services
	Include tech support + security
5.Optimize Pricing Strategy
	Personalized offers for high-paying users
-------------------------------------------------------------------------------------------------
 What I learned from this model?
The most important factors influencing churn were tenure, contract type, and service-related features like tech support and online security.
Customers with shorter tenure and month-to-month contracts showed significantly higher churn risk.
Interestingly, demographic features had very low importance, indicating that churn is more driven by service experience than customer profile.
These insights helped design targeted retention strategies like promoting long-term contracts and improving service offerings.
---------------------------------------
1. Logistic Regression Results — Meaning
Accuracy = 0.76 → similar to Random Forest
Precision = 0.54 → slightly better
Recall = 0.82 ✅ (very strong)
F1 Score = 0.65 → improved balance
ROC-AUC = 0.78 ✅ → good model separability
---------------------------------
FINAL-CONCLUSION :
================
I built both Random Forest and Logistic Regression models to predict customer churn. While Random Forest captured non-linear patterns, Logistic Regression slightly outperformed it in terms of precision, recall, and F1-score. With a recall of ~82%, the model effectively identifies high-risk customers. Additionally, its ROC-AUC score of 0.78 indicates good classification capability. Due to its interpretability and strong performance, Logistic Regression is the preferred model for deployment.


<img width="1393" height="807" alt="Screenshot 2026-04-03 125816" src="https://github.com/user-attachments/assets/262c7968-439a-46e9-b714-98b7a034d3e1" />



<img width="1365" height="777" alt="Screenshot 2026-04-03 125825" src="https://github.com/user-attachments/assets/a84c6aa7-5eeb-4eb3-81e7-4cb3f6173591" />




<img width="1319" height="775" alt="Screenshot 2026-04-03 125835" src="https://github.com/user-attachments/assets/70729e29-7814-4634-8f69-ab8d9c645f1c" />



<img width="1368" height="724" alt="Screenshot 2026-04-03 125842" src="https://github.com/user-attachments/assets/94b6b183-b27c-4b07-bcb7-c58f1c18129f" />

<img width="1354" height="775" alt="Screenshot 2026-04-03 125849" src="https://github.com/user-attachments/assets/201e3bc7-9957-4590-8cf6-443850c9c4aa" />


<img width="1388" height="784" alt="Screenshot 2026-04-03 125900" src="https://github.com/user-attachments/assets/500276c9-665f-48eb-bb11-45fe7af92fc7" />



<img width="1395" height="808" alt="Screenshot 2026-04-03 125909" src="https://github.com/user-attachments/assets/90132789-5dda-4d95-b581-41a8b2fa4188" />




<img width="1339" height="785" alt="Screenshot 2026-04-03 125915" src="https://github.com/user-attachments/assets/eacbd1b9-8136-4520-8cf2-3e91d082e754" />

<img width="1399" height="527" alt="Screenshot 2026-04-03 125922" src="https://github.com/user-attachments/assets/12c48a83-c851-49a6-932f-e9a69a874409" />




<img width="1405" height="813" alt="Screenshot 2026-04-03 125928" src="https://github.com/user-attachments/assets/1e730510-bb3a-4012-a428-569b2882e48d" />




<img width="1403" height="800" alt="Screenshot 2026-04-03 125935" src="https://github.com/user-attachments/assets/62f4cda8-704c-4bdd-b8ef-6e373bc89816" />






<img width="1409" height="788" alt="Screenshot 2026-04-03 125944" src="https://github.com/user-attachments/assets/8d5601c8-e652-418f-9dcc-dd13853bb50b" />



























