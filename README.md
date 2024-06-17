# ML-Predict-Churned-Users
This approach utilizes supervised learning, a branch of machine learning, to predict customer churn. By analyzing customer behavior, the model identifies key indicators that signal a customer's likelihood to churn (cancel their service or stop using a product).
# I.	Introduction
## 1. Context
Customer Churn is when customers stop purchasing/using business's products or service in certain period of time. Customer churn is one critical metric because it's less expensive to retain existing customers than acquire new customers. In this kernel, I'll analyze E-commerce customer churn rate and looking for user patterns whos likely churned. Customer churn rate indicates how many existing customers are not using products-services or switch to business competitors.
## 2. Business question
One ecommerce company has a project on predicting churned users in order to offer potential promotions. An attached file is the dataset that is offered by the company (churn_predict.csv). You will using these dataset to answer below questions:
1.	What are the patterns/behavior of churned users? What are your suggestions to the company to reduce churned users.
2.	Build the Machine Learning model for predicting churned users.
## 3. Dataset
An attached file is the dataset that is offered by the company (churn_predict.csv).
![image](https://github.com/lekhuong0196/ML-Predict-Churned-Users/assets/138196501/1b950b8a-8902-4403-a7c8-ac7536c34f20)
## 4. Method
**Supervised learning with Scikit-learn on Python**

•	Supervised learning, also known as supervised machine learning, is a subcategory of machine learning and artificial intelligence. It is defined by its use of labeled datasets to train algorithms that to classify data or predict outcomes accurately.

•	As input data is fed into the model, it adjusts its weights until the model has been fitted appropriately, which occurs as part of the cross validation process.

•	Supervised learning helps organizations solve for a variety of real-world problems at scale, such as classifying spam in a separate folder from your inbox.
# II.	Proccess
**Step 1: Data Preparation**
1.	Import Libraries and Dataset: Begin by importing the necessary libraries and loading the dataset.
2.	Check for Data Imbalance: Assess the balance of the target variable, which in this case is the "churned" variable. If the dataset is imbalanced, consider techniques to address it later in the process.
3.	Data Wrangling: Perform data cleaning and preprocessing tasks to ensure the data is suitable for modeling. This may include handling missing values, converting data types, and removing duplicates.
4.	Exploratory Data Analysis (EDA): Utilize data visualization tools like Seaborn and Matplotlib to gain insights into the data distribution, identify patterns, and uncover potential relationships between variables.
   
**Step 2: Feature Engineering**
1.	Outlier Detection and Handling: Identify and address outliers in the data using appropriate methods, such as the Interquartile Range (IQR) method.
2.	Missing Value Imputation: Impute missing values with suitable strategies, such as replacing numerical values with the median or using more sophisticated imputation techniques.
3.	Feature Transformation: Transform categorical variables into numerical representations using techniques like one-hot encoding or label encoding.

**Step 3: Model Selection**
1.	Choose Appropriate Models: Select a combination of linear and nonlinear models, such as Logistic Regression, Decision Tree, and Random Forest, to capture the complex relationships in the data.
2.	Consider Model Characteristics: Understand the strengths and weaknesses of each model type. Linear models require careful feature selection, while nonlinear models can handle a wider range of feature types.
3.	Random Forest as Preferred Model: Random Forest is often preferred due to its ability to address overfitting, a common issue with Decision Trees.

**Step 4: Model Training**
1.	Split Data into Training and Testing Sets: Divide the dataset into separate training and testing sets. The training set is used to fit the model, while the testing set is used to evaluate its performance.
2.	Train and Evaluate Models: Train each selected model on the training set and evaluate its performance on the testing set. Use metrics like accuracy, precision, recall, and F1-score to assess the models' predictive power.
3.	Select the Best Model: Based on the evaluation results, choose the model that consistently demonstrates the best performance across various metrics.
# III. MODEL EVALUATION:
**Comments on 3 models:**

**Decision Tree:**

•	Balanced accuracy between the training and test sets is significantly different (1.0 and 0.95), indicating severe overfitting.

**Recommendation:** Not recommended due to overfitting issues.

**Random Forest:**

•	Balanced accuracy between the training and test sets is similar (0.66 and 0.65), suggesting the model effectively captures underlying patterns in the dataset and makes reasonable predictions.
Recommendation: Recommended for its ability to generalize well and provide reliable predictions.

**Logistic Regression:**

•	Achieves an average classification accuracy of around 60% and 64% on both training and test sets (0.60 and 0.64).

**Conclusion:**

Based on the evaluation results, the Random Forest model is the most suitable choice due to its consistently high and similar balanced accuracy scores across training and test sets. This indicates its ability to generalize well and make accurate predictions on unseen data.
# IV. RECOMMENDATIONS
**Based on the analysis of the top predictors of churn, we propose the following recommendations to the business:**
1.	Enhance Customer Tenure: Implement loyalty programs or special discounts for long-term customers to foster brand loyalty and reduce churn.
2.	Prioritize Customer Service: Invest in training and empowering customer service representatives to effectively handle complaints and resolve issues promptly, addressing customer concerns and improving satisfaction.
3.	Targeted Promotions for Cardholders: Offer exclusive promotions and benefits to credit and debit cardholders, as they are more likely to churn compared to non-cardholders.
4.	Gather Customer Feedback: Regularly conduct customer surveys to gather feedback and identify areas for improvement. Addressing customer pain points can significantly reduce churn.
5.	A/B Testing for Optimization: Continuously test and refine marketing campaigns, website features, and customer service interactions using A/B testing to optimize customer experience and increase conversion rates.

**Hyperparameter Tuning:**

By employing hyperparameter tuning techniques, we were able to significantly improve the accuracy of the Random Forest model, from 0.66 to 0.96. This demonstrates the potential of optimizing model parameters to enhance predictive performance.
# V. CONCLUSION
This project involved building three machine learning models, Logistic Regression, Decision Tree, and Random Forest, to predict customer churn. Among the models, the Decision Tree model exhibited the highest balanced accuracy of 0.9178, indicating its strong performance in identifying churned users.

The Decision Tree model's balanced accuracy scores for the training set (1.0) and test set (0.9178) are closely aligned, suggesting minimal overfitting. This is further supported by the favorable results from the confusion matrix and classification report, which indicate overall good model performance.

The project's findings provide valuable insights into customer churn patterns and highlight effective strategies for businesses to retain their valuable customer base.






