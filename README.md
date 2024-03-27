# Customer Churn Predictor Project

![image](https://github.com/spark174/Churn-User-Classifier/assets/90639266/d91e3fe1-92dd-4775-a838-7de7a59ced49)

### Purpose and Goal
The primary objective of this project is to develop a predictive model capable of identifying potential churn customers within a telecommunication company's client base. By accurately predicting which customers are at risk of leaving, the company aims to proactively offer tailored product packages or pricing adjustments to retain these customers. The ultimate goal is to correctly identify the customers that are going to leave our services in the next month. By predicting these users correctly, the company will be able to provide better products & services packages in order to retain the clients. Considering the context of a telecommunications company aiming to predict churn, it's crucial to balance between correctly identifying customers who are likely to churn (recall) and not misclassifying too many loyal customers as potential churners (precision). In the scenario of predicting churn, high recall is essential because it reflects the model's ability to catch a high percentage of actual churn cases. However, this should not come at the expense of precision, where a low precision would mean many loyal customers are mistakenly targeted as churn risks, potentially leading to unnecessary retention efforts and offers, which could be costly and inefficient. 

### Data and Preprocessing
The dataset utilized for this project encompasses a wide range of customer attributes, including demographic information, service usage patterns, and billing details. Initial data preprocessing steps involved cleaning missing values, encoding categorical variables, and normalizing numerical features to ensure optimal model performance.

### Model Selection and Evaluation
To address the churn prediction problem, we explored several machine learning models, including Logistic Regression, Random Forest, Support Vector Machine (SVM), Gradient Boosting, and Neural Networks. Each model's performance was rigorously evaluated using precision, recall, F1-score, and accuracy metrics, with a particular focus on the precision-recall trade-off to balance the identification of churn customers against the risk of false positives.

### Model Performance and Insights
The Random Forest model emerged as the most effective, demonstrating superior performance across all evaluation metrics. This model's ability to accurately identify churn customers, combined with its relatively lower rate of false positives, makes it particularly suited for deployment in a customer retention strategy. Furthermore, the feature importance analysis provided by the Random Forest model offers valuable insights into the key factors influencing customer churn, guiding the company in tailoring its retention efforts more effectively.

### Visualization and Interpretation
To aid in the interpretation of model performances and the underlying decision-making processes, we utilized various visualization techniques. Precision-recall curves were generated for each model to illustrate the trade-off between precision and recall at different thresholds. For the Neural Network model, a weights plot was created to visualize the influence of each feature on the model's predictions, offering a glimpse into the neural network's learning process.

### Conclusion and Future Work
The Random Forest model's superior performance and insightful feature importance analysis make it the preferred choice for predicting customer churn in the telecommunication industry. By integrating this predictive model into its customer retention strategies, the company can more effectively identify at-risk customers and take proactive measures to retain them. Moving forward, further enhancements to the model could involve exploring more advanced machine learning techniques and incorporating additional data sources to refine its predictive accuracy.

### Description of data

**CustomerID**: A unique ID that identifies each customer.

**Coun**t: A value used in reporting/dashboarding to sum up the number of customers in a filtered set.

**Country**: The country of the customer’s primary residence.

**State**: The state of the customer’s primary residence.

**City**: The city of the customer’s primary residence.

**Zip Code**: The zip code of the customer’s primary residence.

**Lat Long**: The combined latitude and longitude of the customer’s primary residence.

**Latitude**: The latitude of the customer’s primary residence.

**Longitude**: The longitude of the customer’s primary residence.

**Gender**: The customer’s gender: Male, Female

**Senior Citizen**: Indicates if the customer is 65 or older: Yes, No

**Partner**: Indicate if the customer has a partner: Yes, No

**Dependents**: Indicates if the customer lives with any dependents: Yes, No. Dependents could be children, parents, 
grandparents, etc.

**Tenure Months**: Indicates the total amount of months that the customer has been with the company by the end of the quarter 
specified above.

**Phone Service**: Indicates if the customer subscribes to home phone service with the company: Yes, No

**Multiple Lines**: Indicates if the customer subscribes to multiple telephone lines with the company: Yes, No

**Internet Service**: Indicates if the customer subscribes to Internet service with the company: No, DSL, Fiber Optic, Cable.

**Online Security**: Indicates if the customer subscribes to an additional online security service provided by the company: 
Yes, No

**Online Backup**: Indicates if the customer subscribes to an additional online backup service provided by the company: Yes, No

**Device Protection**: Indicates if the customer subscribes to an additional device protection plan for their Internet 
equipment provided by the company: Yes, No

**Tech Support**: Indicates if the customer subscribes to an additional technical support plan from the company with reduced 
wait times: Yes, No

**Streaming TV**: Indicates if the customer uses their Internet service to stream television programing from a third party 
provider: Yes, No. The company does not charge an additional fee for this service.

**Streaming Movies**: Indicates if the customer uses their Internet service to stream movies from a third party provider: Yes, 
No. The company does not charge an additional fee for this service.

**Contract**: Indicates the customer’s current contract type: Month-to-Month, One Year, Two Year.

**Paperless Billing**: Indicates if the customer has chosen paperless billing: Yes, No

**Payment Method**: Indicates how the customer pays their bill: Bank Withdrawal, Credit Card, Mailed Check

**Monthly Charge**: Indicates the customer’s current total monthly charge for all their services from the company.

**Total Charges**: Indicates the customer’s total charges, calculated to the end of the quarter specified above.

**Churn Label**: Yes = the customer left the company this quarter. No = the customer remained with the company. Directly 
related to Churn Value.

**Churn Value**: 1 = the customer left the company this quarter. 0 = the customer remained with the company. Directly related 
to Churn Label.

**Churn Score**: A value from 0-100 that is calculated using the predictive tool IBM SPSS Modeler. The model incorporates 
multiple factors known to cause churn. The higher the score, the more likely the customer will churn.

**CLTV**: Customer Lifetime Value. A predicted CLTV is calculated using corporate formulas and existing data. The higher the 
value, the more valuable the customer. High value customers should be monitored for churn.

**Churn Reason**: A customer’s specific reason for leaving the company. Directly related to Churn Category.

### Questions and Feedback
For any questions or feedback regarding this project, please feel free to contact sspark2@andrew.cmu.edu. Your insights and suggestions are highly valued as we strive to continuously improve the models and strategies.
