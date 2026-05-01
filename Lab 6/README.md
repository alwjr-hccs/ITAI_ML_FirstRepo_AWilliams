Instructions: Answer the following questions in this markdown cell.

In your own words, what is the key difference between a regression problem and a classification problem?
Regression predicts a continuous numerical value (e.g., fare, temperature). Classification predicts a discrete category or class label (e.g., survived vs. not survived).

The LinearRegression model has an attribute called .coef_. After you train the model, print lr_model.coef_. What do these numbers represent?
The values in lr_model.coef_ are the learned slopes (weights) for each feature. They quantify how much the target changes, on average, for a one-unit increase in the corresponding feature while holding other features constant.

Why did we use mean_squared_error to evaluate the regression model but accuracy_score for the classification model? Why wouldn't accuracy be a good metric for the fare prediction task?
mean_squared_error measures the average squared numerical difference between predicted and actual values, which is appropriate for continuous targets. accuracy_score measures the fraction of correct class labels, which is appropriate for classification. Accuracy isn't suitable for fare prediction because fares are continuous — using accuracy would require arbitrary discretization and would not reflect the magnitude of prediction errors (e.g., being off by 
5 would both count as "incorrect").
