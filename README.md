### Fraudulent Transaction Prediction
#### Business Context
To develop a model for predicting fraudulent transactions for a financial company and use insights from the model to develop an actionable plan.
#### Problem Domain - "Financial Industry"
Fraud transaction detection is of utmost importance in the financial industry due to the potential financial losses, reputational damage, and customer trust implications caused by fraudulent activities.
#### Process
Began by cleaning up the data, then explored and understood the data. In the data, there were neither duplicates nor missing values that needed to be handled. There was strong correlation among many independent variables. In contrast to regression problems, classification problems do not necessarily need to address multicollinearity as primary concern. However, it was addressed by some feature engineering and the removal of pointless columns (justified) because it may increase the risk of overfitting. 
##### Models Built :
###### Logistic Regression
###### Decision Tree Classifier
To lessen the amount of false positives is the main goal. Despite the importance of tackling all fraud cases, an extremely high false positive rate may result in operational inefficiencies.
The recall and precision scores were very low, despite the fact that Logistic could provide acceptable accuracy.
Even XG Boost took a lot of processing power and was unable to provide fewer false positives.
However, the Decision Tree Classifier performed admirably in this instance, achieving 99% accuracy for both the train and validation datasets.
Thereby assigning class weights to address class imbalance, as the model may be biassed towards forecasting the majority class and underperform on the minority class (fraudulent transactions) if the dataset is unbalanced and the majority class (non-fraudulent transactions) dominates the data. herefore, Decision Tree is constructed with certain manually provided class weights in order to address class imbalance and improve false positives without overfitting or underfitting. 
Used Accuracy, Recall, Precision, F1 Score and ROC AUC Score, as evaluation metrics, and developed a promising model.
### Thank You
