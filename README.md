# Propensity-Model-V2
Model prospect propensity to accept credit line marketing offers.
1. Objective
Develop a data-driven model to predict the likelihood of prospect acquisition for credit line marketing offers, enabling more efficient targeting and improving campaign ROI.
2. Business Context
The marketing team wanted to reduce acquisition costs by identifying prospects most likely to respond to promotional credit line offers.
This model provides a propensity score for each prospect, ranking them by their probability of conversion.
3. Data Sources
Customer demographic data: age, income, location, tenure, etc.
Transactional data: spending patterns, credit usage, payment history.
Marketing interactions: previous campaign responses, contact frequency.
External data (optional): credit bureau score, regional economic factors.

4. Data Preparation and Modeling
Data Cleaning & Feature Engineering
Handled missing values and standardized numeric variables.
Encoded categorical features (e.g., region, channel).
Created aggregated behavioral features such as:
Average monthly spend
Number of credit inquiries
Recent campaign interactions
Labeled data with a binary target: 1 = Accepted offer, 0 = Did not accept.
Modeling Approach
Split data into training (70%) and test (30%) sets.
Evaluated multiple algorithms:
Logistic Regression
Random Forest
XGBoost
Selected XGBoost for best balance of precision and interpretability.
Tuned hyperparameters using GridSearchCV and cross-validation.
Model Output
Generated propensity scores (0–1) for each prospect.
Used threshold optimization to classify high-propensity leads.

Results in a Glips 

Monthly digital activityin and retention relationship suggests the following:
1. Higher Digital Engagement → Higher Retention
Customers who actively use digital channels (website, mobile app, online services) are more likely to:
- Stay longer with the bank,
- Be more satisfied, and
- Engage with multiple products.

Interpretation:
Digital interaction strengthens the customer relationship; every login or online action increases familiarity and reduces churn risk.
insight:
“Customers with more than 10 digital interactions per month have a 40% higher 6-month retention rate than low-activity users.”

2. Mobile App Usage as a Retention Predictor
Frequent logins indicate trust and dependency on the digital platform.
This variable becomes a strong predictor in your propensity model for retention or offer acceptance.
Interpretation:
“Mobile login frequency can be used as a key feature in the propensity model — customers logging in weekly are twice as likely to respond to a credit line offer compared to inactive users.”

1. Model Behavior
The model learns that:
Higher digital engagement scores and mobile logins correlate with higher propensity to stay (retain) or accept offers.
Low digital activity signals potential churn or low responsiveness.

2. Actionable Results
High Propensity Segment (Top 20%):
Customers highly engaged digitally — prioritize for cross-sell and premium offers.
Example: 0.85–0.95 probability range
Medium Propensity Segment (20–60%):
Moderate engagement — target with personalized nudges (e.g., app feature highlights or usage incentives).
Low Propensity Segment (Bottom 40%):
Low login frequency or digital inactivity — consider retention campaigns or educational outreach.

3. Business Takeaway
Each additional monthly login increases retention likelihood by X%.
Customers with consistent mobile engagement show 2–3× higher response rates to digital offers.
By targeting the top propensity decile, marketing ROI improved (for example) +25%, and retention loss reduced –15%.


