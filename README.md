# Customer-Behavior-Prediction
You are provided with more than 1 year of customer product data. The objective is to predict what accounts a customer will acquire in the next month, 2016-05. The dataset is split into training and tests sets. You will use the training data, ranging from 2015-01 to 2016-04, to build your model. You will make your predictions on 2016-05, which can be found in the test set. This dataset doesn’t contain any real bank data.


GRM: Credit Sciences Business Case 
Overview
You are provided with more than 1 year of customer product data. The objective is to predict what accounts a customer will acquire in the next month, 2016-05. The dataset is split into training and tests sets. You will use the training data, ranging from 2015-01 to 2016-04, to build your model. You will make your predictions on 2016-05, which can be found in the test set. This dataset doesn’t contain any real bank data.
The dataset contains monthly information for the following:
1) Customer identifiers
2) Customer characteristics: demographic, geographic, etc.
3) Customer's accounts
Submission Files
For every user in 2016-05, you must predict a ‘;’ delimited list of the products they added.  Please submit your prediction in the following format:
cust_id, added_products
12345, savings_account
67821, mortgage; e_account
69405, payroll_account; pensions
….,…



Please name the file: ‘{your_name}_predictions.csv’
In addition, we ask you submit your code including comments on the approach taken.
Evaluation
Submissions are evaluated according to the Mean Average Precision @ 7 (MAP@7):
 
where |U| is the number of rows (users in two time points), P(k) is the precision at cut-off k, n is the number of predicted products, and m is the number of added products for the given user at that time point. If m = 0, the precision is defined to be 0. Please note that the order of your predictions for each customer matters. Your predictions must be arranged in descending order. In other words, the products you predict a customer will add should be rank ordered in descending order by their likelihood of being added.
For a detailed explanation of how the MAP evaluation works, please visit this link:
http://sdsawtelle.github.io/blog/output/mean-average-precision-MAP-for-recommender-systems.html.
Suggestions
1.	While obtaining a good evaluation is important, we are more interested in the approach that you take to make your predictions.  Writing detailed explanations along with your code will allow for a more fruitful discussion during the interview process.
2.	Provide a brief summary at the end to explain the additional steps you could have taken to increase your model(s) ability to make correct predictions.
3.	Which part of the business process could you apply this predictive model to?







