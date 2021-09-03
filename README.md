# Credit Card Fraud Detection - Italian Bank

Credit cards play a significant role in today's economy, both on a small and on a larger scale: they are used in everyday shopping as well as in global business activities. Just as the use of credit cards offers great benefits, likewise the financial damage from fraudulent activities can be huge. Many machine learning techniques have been proposed to tackle the growth of credit card fraud; each has its own advantages and disadvantages, but all of these techniques share the same objective - which is indeed that of preventing and avoiding credit card fraud. In recent years there has been a rapid increase in the rate of fraudulent activity, causing considerable financial loss to many organisations, businesses and government agencies. Fraud rates are set to increase in the future, and it’s for this that many researchers have focused on fraud detection using advanced machine learning techniques. However, credit card fraud detection is not an easy task, mainly because of two reasons:

1.	Fraudulent behaviour changes with each attempt.
2.	The dataset is highly imbalanced, i.e. the frequency of legitimate transactions is significantly higher than fraudulent transactions.

When providing input data of a highly imbalanced class distribution to the predictive model,
the model tends to be biased towards the majority samples. As a result, it will be prone to misrepresenting a fraudulent transaction as a genuine transaction. To tackle this problem, I have been implemented data-level approach on the one hand (with different resampling methods such as undersampling, oversampling) and hybrid strategies on the other, with an algorithmic approach; from here, ensemble models like Bagging and Boosting have been applied to a highly skewed dataset containing 5’442’906 transactions owned by a large Italian bank, the identity of which will be omitted for privacy reasons. Out of these transactions, only 47’662 transactions are labelled as fraudulent. Feature selection techniques such as correlation and Isolation Forest and Outlier Detection techniques such as IQR method and Extra Tree Classifier were used to make the data less heavy. Predictive models such as Logistic Regression, XGBoost, Random Forest and Easy Ensemble have been employed to predict if a transaction is fraudulent or genuine. The objective of the thesis was to minimise both false negatives and false positives by trying to find an acceptable trade-off and measuring performance.

The performance of the model is evaluated based on ROC AUC score, and G-Mean metric. 
The best algorithm was the Random Forest, on the dataset obtained with Undersampling. These models were selected for a better trade-off between cost and performance compared to the others. By using the pre-processed dataset with a correlation features selection, we obtained a ROC AUC score of 0.8715 and a G-mean of 0.8699 and with the Extra Tree a ROC AUC score of 0.8923 and a G-mean of 0.8524.
