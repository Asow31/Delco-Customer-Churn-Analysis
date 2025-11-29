Delco Customer Churn Analysis

Dashboard link
You can view the full interactive dashboard here:
https://public.tableau.com/app/profile/abdoul.sow4068/viz/CustomerChurnAnalysisDashboard_17642240688170/TelcoCustomerChurnAnalysisDashboard?publish=yes

This project looks at customer churn for Delco. My goal was to understand why some customers leave, what patterns stand out in the data, and whether a basic machine-learning model could help predict churn. 

Tools Used
	•	Python (Pandas, NumPy)
	•	scikit-learn
	•	Jupyter Notebook / VS Code
	•	Tableau
	•	Excel/CSV files

1. Getting Familiar With the Data

Before running any model, I spent time looking at the structure of the dataset. It included customer demographics, contract information, billing details, payment methods, and the churn label. I checked the distributions, correlations, and simple statistics to see where the biggest differences were.

The variables that stood out the most were:
	•	contract type
	•	tenure
	•	monthly charges
	•	payment method

2. Preparing the Data

I cleaned up missing values, fixed inconsistent entries, encoded the categorical columns, and then split the dataset into training and testing sets. Nothing complicated —just the essential steps to get the data ready.


3. Exploring the Data

This part showed the clearest patterns in customer behavior.

Contract Type

Month-to-month customers left much more often than customers on yearly contracts. Short contracts make it easier to cancel quickly, which explains the difference.

Tenure

New customers had the highest churn rates. Once a customer stayed long enough, they were far less likely to leave.

Monthly Charges

Customers paying higher monthly fees churned more frequently. There seems to be a connection between high cost and dissatisfaction, especially early in their service.

Payment Method

Some payment methods, like electronic check, had noticeably higher churn compared to automatic payments. Billing habits appear to be a useful signal.


4. Machine Learning Model

I tried a few simple classification models, including logistic regression and tree-based methods.
I checked accuracy, precision/recall, and the confusion matrix to judge how well they performed.

Across different models, the most important features were:
	•	contract type
	•	tenure
	•	monthly charges
	•	payment behavior

5. Visualizations

I built a dashboard that highlights:
	•	overall churn rate
	•	churn by contract type
	•	churn by monthly charges
	•	churn by customer segment

The goal was to present the results in a simple way for someone who doesn’t work with data daily.

6. Main Takeaways
	•	Most churn happens within the first few months.
	•	Customers on month-to-month contracts are the riskiest group.
	•	Higher monthly charges make churn more likely.
	•	Payment method can signal potential churn issues.

7. Practical Recommendations
	•	Provide better onboarding for new customers.
	•	Offer incentives to switch to longer-term contracts.
	•	Review pricing for higher-paying customers.
	•	Encourage automatic payment methods to reduce billing-related churn.
