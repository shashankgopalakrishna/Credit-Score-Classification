# Credit-Score-Classification

The classification of the credit score is the crucial part in the financial organizations to calculate the individuals credit worthiness. The credit score evaluation of individual creditworthiness used by the financial banking sectors in determining to sanction the loan amount eligibility for customers. The main idea of this classification lies in its ability to condense complex financial histories into actionable information, enabling institutions to predict the creditworthiness of individuals with accuracy. By analyzing past repayment behaviors and financial activities, credit scoring systems facilitate the partition of customers into distinct categories, ranging from highly reliable to those presenting elevated risks. These categories, labeled as ”good,” ”standard,” and ”poor,” act as guiding markers for lenders, helping them make wise lending decisions.<br/>
<br/>
We will evaluate the performance of the each models trained for credit card classification based on the provided dataset. Will discuss the results obtained from each model and provide insights into their predictive capabilities.<br/>

### A. Linear Regression
• The linear regression model showed poor performance, as indicated by a high mean squared error 0.44 (MSE) and negligible R-squared value. This suggests that the model failed to effectively capture the relationship between predictors and the target variable.<br/>
• Linear regression assumes a linear relationship between the independent and dependent variables. However, in the context of credit card classification, where the relationship may be nonlinear and complex, linear regression may not be the most suitable model.<br/>
• Given its poor performance, it’s advisable to explore more advanced modeling techniques that can capture nonlinear relationships and interactions in the data.<br/>
<br/>
Mean Squared Error (MSE): 0.4476533893319599<br/>
R-squared (R2): -0.00029430073231373477<br/>

### B. Logistic Regression
• The logistic regression model achieved an accuracy of 54.10%, slightly better than random guessing. However, its precision, recall, and F1-score indicate that it struggled to accurately classify credit card classifications.<br/>
• Logistic regression is a linear model used for binary classification. While it can provide probability estimates for class membership, it may not be suitable for capturing complex relationships in the data.<br/>
• Considering its limited performance, alternative classification models should be explored to improve predictive accuracy and reliability.<br/>

Accuracy: 0.5410339532502986<br/>
Precision: 0.2927177385696463<br/>
Recall: 0.5410339532502986<br/>
F1-score: 0.37989784449882563<br/>

### C. Decision Tree Classifier
• The decision tree classifier outperformed linear and logistic regression, achieving an accuracy of 76.32% with balanced precision, recall, and F1-score. It effectively captured nonlinear relationships between predictors and the target variable.<br/>
• Decision trees are non-linear models that partition the feature space into distinct regions based on the predictors’ values. They are capable of capturing complex decision boundaries and interactions among features.<br/>
• The decision tree classifier shows promise for credit card classification tasks. Further optimization and finetuning of hyperparameters could potentially enhance its performance even more.<br/>

Accuracy: 0.762497867258147<br/>
Precision: 0.7645315214212544<br/>
Recall: 0.762497867258147<br/>
F1-score: 0.7615683460773391<br/>

### D. Random Forest Classifier
• The random forest classifier performed similarly to the decision tree model, with an accuracy of 74.37% and balanced precision, recall, and F1-score. It leveraged ensemble learning to make robust predictions..<br/>
• Random forests are an ensemble of decision trees that aggregate predictions from multiple trees to improve generalization and reduce over-fitting. They are robust against
noise and outliers and can handle high-dimensional data well.<br/>
• The random forest classifier offers a reliable and accurate solution for credit card classification tasks. Further experimentation with different ensemble methods or model architectures could potentially yield even better results.<br/>

Accuracy: 0.7417676164477052<br/>
Precision: 0.7417951435630697<br/>
Recall: 0.7417676164477052<br/>
F1-score: 0.7415625276923002<br/>

## PREDICTIONS ON TEST.CSV
Based on the evaluation results, both the decision tree classifier and random forest classifier outperformed linear and logistic regression for credit card classification.
a) Predictions: The predicted credit card classifications from the chosen model (either decision tree or random forest) on the test.csv dataset can provide valuable insights for financial institutions.<br/>
b) Application: These predictions can assist in assessing the creditworthiness of applicants, managing risk, and making informed decisions about lending. By classifying applicants
into different credit score categories, financial institutions can tailor their lending practices and mitigate potential default risks.<br/>
c) Recommendation: It’s important to monitor the models’ performance over time and update them as needed to ensure accurate predictions and effective risk management. Regular evaluation and validation of the models against new data will help maintain their predictive accuracy and reliability in real-world applications.<br/>

<img src="https://github.com/shashankgopalakrishna/Credit-Score-Classification/assets/143437355/92dd309c-ddb5-4b6b-a546-ed94ce59d88d" alt="drawing" width="350"/>

Fig. 1. Predicted Credit score on test.csv

## CONCLUSION

The analysis reveals the significant positive correlation between Annual Income and Credit Score. As the Annual Income increases, there is a tendency for the Credit Score to increase as well. This tells that individuals with higher incomes tend to have better credit scores.<br/>

a) Linear Regression model shows poor performance, with a high mean squared error (MSE) and negligible R-squared value. It fails to effectively capture the relationship between
predictors and the target variable.<br/>
b) Logistic Regression model achieves an accuracy of 54.10%, indicating slightly better performance than random guessing. However, its precision, recall, and F1-score suggest that it struggles to accurately classify credit card classifications.<br/>
c) Decision Tree Classifier outperforms linear and logistic regression, achieving an accuracy of 76.32% with balanced precision, recall, and F1-score. It effectively captures nonlinear relationships between predictors and the target variable.<br/>
d) Random Forest Classifier performs similarly to the decision tree model, with an accuracy of 74.37% and balanced precision, recall, and F1-score. It leverages ensemble learning to make robust predictions.<br/>

![image](https://github.com/shashankgopalakrishna/Credit-Score-Classification/assets/143437355/10d1724e-07aa-416c-9222-74eb9cf9952e)
Fig. 2. Train and test accuracy of the models

The conclusion based on the evaluation results, both the decision tree classifier and random forest classifier outperform linear and logistic regression for credit card classification. The decision tree and random forest models achieve higher accuracy and balanced precision, recall, and F1-score, indicating better overall performance. These models are suitable for predicting credit card classifications, with the decision tree model being slightly superior in terms of accuracy.<br/>
