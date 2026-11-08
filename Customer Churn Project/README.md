# Customer Churn Prediction

## 1. Project Overview
This project uses machine learning classification algorithms to predict customer churn in the telecommunications industry. The objective is to identify customers who are likely to leave a service provider and understand the factors associated with their decisions.

## 2. Dataset
- Dataset: Telco Customer Churn
- Problem Type: Binary Classification
- Target Variable: `Churn`
- Classes: `Yes` (customer churned) and `No` (customer retained)

The dataset contains customer demographics, account information, subscribed services, contract details, and billing information.

## 3. Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn
- Google Colab

## 4. Project Workflow

### Exploratory Data Analysis (EDA)
- Examined the dataset structure, data types, and statistical summaries.
- Analyzed the distribution of churn and non-churn customers.
- Visualized relationships between churn and customer characteristics.

### Data Cleaning and Preprocessing
- Checked for missing values and data inconsistencies.
- Converted `TotalCharges` into a numeric format.
- Prepared categorical and numerical features for model training.

### Feature Analysis
Investigated the relationships between customer churn and:
- Contract type
- Customer tenure
- Monthly charges
- Payment method
- Internet service
- Online security
- Technical support

### Model Training
Trained and compared seven classification algorithms on the original dataset.

### Handling Class Imbalance
Applied SMOTEENN to the training data to investigate whether resampling improves classification performance.

### Model Evaluation
Compared model performance using:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix

## 5. Model Evaluation
Models were evaluated on the original imbalanced dataset and compared with models trained using SMOTEENN-resampled training data.

The final model should be selected based on its performance on an untouched test set, considering precision, recall, and F1-score alongside accuracy.

Note: Refer to the notebook for the latest evaluation results.

## 6. Key Findings
Exploratory analysis identified several customer characteristics associated with churn:
- Customers with month-to-month contracts showed higher churn.
- Customers with shorter tenure were more likely to leave.
- Customers without online security or technical support showed higher churn.
- Churn patterns varied across payment methods and internet service types.

These findings describe associations in the dataset and do not necessarily establish causation.

## 7. Key Learnings
- Exploratory Data Analysis and data visualization
- Data cleaning and preprocessing
- Categorical feature encoding
- Classification model comparison
- Class imbalance and SMOTEENN
- Model evaluation using multiple performance metrics

## 8. Future Improvements
- Perform hyperparameter tuning.
- Compare ROC-AUC and precision-recall performance.
- Analyze feature importance.
- Validate models using cross-validation.
- Develop an interactive application for churn prediction.

## 9. Conclusion
This project demonstrates an end-to-end machine learning workflow for customer churn analysis, from data exploration and preprocessing to model training and evaluation. It also investigates the impact of class imbalance handling on classification performance.