# Wincor Customer Churn Analysis
### Prepared by [Ekaterina Serbina]([https://github.com/your_username](https://github.com/serbinaekaterinai))

Wincor, an Internet Service Provider (ISP), is dedicated to delivering superior customer satisfaction. However, churn - when customers decide to terminate their subscriptions or switch to a different service provider - is a persisting challenge. This project aims to analyze customer data to understand the primary reasons behind churn and predict potential churners to proactively implement retention strategies.

## Business Problem
Reducing churn rates is crucial for maintaining revenue stability and enhancing the company's reputation. Predicting which customers might churn and understanding why they might do so allows Wincor to take proactive measures to retain them. By identifying and addressing the reasons leading to customer dissatisfaction, Wincor can improve its services and overall customer satisfaction.

## Data Insights
The dataset contains information on 7,043 customers, including demographics, account details, and service subscriptions. Some key observations from the data:
- The data is slightly imbalanced, with 5,163 non-churning and 1,869 churning customers.
- The dataset comprises 21 columns, detailing aspects such as contract type, monthly charges, total charges, and the type of services opted by the customer.

## Methodology
1. **Data Preprocessing**: 
   - One-Hot encoding was employed to handle categorical variables.
   - Data was scaled for better model performance.
   - SMOTE (Synthetic Minority Over-sampling Technique) was used to address the imbalanced data issue.

2. **Modeling**:
   - **Logistic Regression**: Served as the baseline model. It achieved a recall of approximately 78% on the test set, indicating its ability to capture a significant proportion of potential churners.
   - **Decision Trees**: An initial decision tree model displayed signs of overfitting. Further hyperparameter tuning improved performance.

3. **Evaluation Metrics**:
   - Given the business context, recall was the prioritized metric as it indicates the model's ability to identify potential churners.
   - Additional metrics such as accuracy, precision, and the F1 score provided a comprehensive view of model performance.

4. **Feature Importance**:
   - Tenure, total charges, contract type, and monthly charges emerged as some of the most influential factors determining customer churn.

## Key Findings & Recommendations
1. **Promote Longer-Term Contracts**: Long-term contracts, especially one-year and two-year plans, were inversely related to churn. Customers should be incentivized to opt for longer durations.
2. **Review Pricing Strategies**: Higher monthly charges correlate with increased churn. Introducing competitive pricing or value bundles can aid retention.
3. **Diversify Payment Options**: Customers using electronic checks as a payment method displayed a higher propensity to churn. Introducing varied and convenient payment methods can enhance customer experience.
4. **Enhance Fiber Optic Internet Service**: The analysis revealed a higher likelihood of churn among fiber optic service users. Efforts should be made to address this, possibly by improving service quality or addressing specific concerns related to this service type.

## Future Work
- **Predictive Analytics for Personalized Interventions**: Use advanced ML techniques to recommend specific retention actions tailored to individual customer profiles.
- **Customer Sentiment Analysis**: Implement sentiment analysis on customer feedback and social media interactions to comprehend the emotional reasons behind churn.
- **Leveraging Advanced Data Sources**: Integrate data like customer interaction logs, support ticket data, and industry trends to provide a holistic understanding of churn behavior.

## Conclusion
By leveraging machine learning and data analysis, Wincor can proactively identify customers at risk of churning and implement tailored strategies to retain them. Implementing the recommendations from this analysis can lead to increased customer satisfaction, reduced churn rates, and enhanced business sustainability.

## Additional Materials

Please review our full analysis in our [Jupyter Notebook](https://github.com/serbinaekaterinai/Wincor_Churn_analysis/blob/main/Project%20Wincor.ipynb) or our [presentation](https://github.com/serbinaekaterinai/Wincor_Churn_analysis/blob/main/Project%20Wincor%20Presentation.pdf) .
