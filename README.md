Bank Marketing Prediction – Machine Learning Models
📌 Overview
This project focuses on predicting whether a client will subscribe to a term deposit using the Bank Marketing dataset. The dataset comes from real marketing campaigns of a Portuguese banking institution and includes both numerical and categorical client information.

The main objective is to apply machine learning classifiers to build predictive models and evaluate their performance using standard metrics.

📊 Dataset
Source: Kaggle – Bank Marketing Dataset

Records: ~11,000 rows

Features: Includes client demographics (age, job, marital status, education), financial details (balance, loan, housing), and campaign-related features (previous contact, days passed, outcome).

Target Variable:

deposit → Whether the client subscribed to a term deposit (yes or no).

⚙️ Methodology
Data Preprocessing

Handled categorical variables using encoding (One-Hot/Label Encoding).

Standardized numerical variables where required.

Train-test split performed for evaluation.

Models Implemented

Logistic Regression

Support Vector Machines (SVC)

Random Forest Classifier

Neural Network (MLPClassifier)

Model Selection

Used GridSearchCV for hyperparameter tuning.

Employed cross-validation to improve generalization.

Feature selection explored with RFECV.

Evaluation Metrics

Accuracy

F1-Score

ROC-AUC

Visualization

Seaborn/Matplotlib plots for feature analysis.

Plotly for interactive insights.

📈 Results & Insights
Random Forest and Neural Networks generally performed better than simple linear models.

Imbalance in the dataset required careful metric evaluation beyond accuracy (F1-score and ROC-AUC were more reliable).

Campaign success was strongly correlated with features such as duration of last call, contact type, and past outcomes.

🎯 Key Takeaways
The project demonstrates end-to-end ML lifecycle: data acquisition → preprocessing → model training → hyperparameter tuning → evaluation.

Ensemble methods like Random Forest outperform basic models on structured bank marketing data.

Proper evaluation metrics (ROC-AUC, F1) are crucial when working with imbalanced classification tasks.

🚀 Future Work
Explore XGBoost and LightGBM for improved performance.

Apply SMOTE or class-weight balancing for better handling of imbalance.

Deploy the final model as a Flask / FastAPI web service.


