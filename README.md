# Credit-Score-Classification

The classification of the credit score is the crucial part in the financial organizations to calculate the individuals credit worthiness. The credit score evaluation of individual creditworthiness used by the financial banking sectors in determining to sanction the loan amount eligibility for customers. The main idea of this classification lies in its ability to condense complex financial histories into actionable information, enabling institutions to predict the creditworthiness of individuals with accuracy. By analyzing past repayment behaviors and financial activities, credit scoring systems facilitate the partition of customers into distinct categories, ranging from highly reliable to those presenting elevated risks. These categories, labeled as ”good,” ”standard,” and ”poor,” act as guiding markers for lenders, helping them make wise lending decisions.

A. Linear Regression
• The linear regression model showed poor performance, as indicated by a high mean squared error 0.44 (MSE) and negligible R-squared value. This suggests that the model failed to effectively capture the relationship between predictors and the target variable.
• Linear regression assumes a linear relationship between the independent and dependent variables. However, in the context of credit card classification, where the relationship may be nonlinear and complex, linear regression may not be the most suitable model.
• Given its poor performance, it’s advisable to explore more advanced modeling techniques that can capture nonlinear relationships and interactions in the data.

Mean Squared Error (MSE): 0.4476533893319599
R-squared (R2): -0.00029430073231373477

B. Logistic Regression
• The logistic regression model achieved an accuracy of 54.10%, slightly better than random guessing. However, its precision, recall, and F1-score indicate that it struggled to accurately classify credit card classifications
• Logistic regression is a linear model used for binary classification. While it can provide probability estimates for class membership, it may not be suitable for capturing complex relationships in the data.
• Considering its limited performance, alternative classification models should be explored to improve predictive accuracy and reliability.
Accuracy: 0.5410339532502986
Precision: 0.2927177385696463
Recall: 0.5410339532502986
F1-score: 0.37989784449882563

C. Decision Tree Classifier
• The decision tree classifier outperformed linear and logistic regression, achieving an accuracy of 76.32% with balanced precision, recall, and F1-score. It effectively captured nonlinear relationships between predictors and the target variable.
• Decision trees are non-linear models that partition the feature space into distinct regions based on the predictors’ values. They are capable of capturing complex decision boundaries and interactions among features.
• The decision tree classifier shows promise for credit card classification tasks. Further optimization and finetuning of hyperparameters could potentially enhance its performance even more.
Accuracy: 0.762497867258147
Precision: 0.7645315214212544
Recall: 0.762497867258147
F1-score: 0.7615683460773391

D. Random Forest Classifier
• The random forest classifier performed similarly to the decision tree model, with an accuracy of 74.37% and balanced precision, recall, and F1-score. It leveraged ensemble learning to make robust predictions..
• Random forests are an ensemble of decision trees that aggregate predictions from multiple trees to improve generalization and reduce over-fitting. They are robust against
noise and outliers and can handle high-dimensional data well.
• The random forest classifier offers a reliable and accurate solution for credit card classification tasks. Further experimentation with different ensemble methods or model architectures could potentially yield even better results.
Accuracy: 0.7417676164477052
Precision: 0.7417951435630697
Recall: 0.7417676164477052
F1-score: 0.7415625276923002

## PREDICTIONS ON TEST.CSV
Based on the evaluation results, both the decision tree classifier and random forest classifier outperformed linear and logistic regression for credit card classification.
a) Predictions: The predicted credit card classifications from the chosen model (either decision tree or random forest) on the test.csv dataset can provide valuable insights for financial institutions.
b) Application: These predictions can assist in assessing the creditworthiness of applicants, managing risk, and making informed decisions about lending. By classifying applicants
into different credit score categories, financial institutions can tailor their lending practices and mitigate potential default risks.
c) Recommendation: It’s important to monitor the models’ performance over time and update them as needed to ensure accurate predictions and effective risk management. Regular evaluation and validation of the models against new data will help maintain their predictive accuracy and reliability in real-world applications.

Fig. 1. Predicted Credit score on test.csv

## CONCLUSION

The analysis reveals the significant positive correlation between Annual Income and Credit Score. As the Annual Income increases, there is a tendency for the Credit Score to increase as well. This tells that individuals with higher incomes tend to have better credit scores.

a) Linear Regression model shows poor performance, with a high mean squared error (MSE) and negligible R-squared value. It fails to effectively capture the relationship between
predictors and the target variable.
b) Logistic Regression model achieves an accuracy of 54.10%, indicating slightly better performance than random guessing. However, its precision, recall, and F1-score suggest that it struggles to accurately classify credit card classifications.
c) Decision Tree Classifier outperforms linear and logistic regression, achieving an accuracy of 76.32% with balanced precision, recall, and F1-score. It effectively captures nonlinear relationships between predictors and the target variable.
d) Random Forest Classifier performs similarly to the decision tree model, with an accuracy of 74.37% and balanced precision, recall, and F1-score. It leverages ensemble learning to make robust predictions.

Fig. 2. Train and test accuracy of the models

The conclusion based on the evaluation results, both the decision tree classifier and random forest classifier outperform linear and logistic regression for credit card classification. The decision tree and random forest models achieve higher accuracy and balanced precision, recall, and F1-score, indicating better overall performance. These models are suitable for predicting credit card classifications, with the decision tree model being slightly superior in terms of accuracy.
