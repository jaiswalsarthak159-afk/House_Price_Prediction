# House_Price_Prediction🏠 House Price Prediction
A machine learning project predicting house sale prices using the Kaggle House Prices Competition dataset. This is my second end-to-end ML project, built after completing Kaggle's Intermediate Machine Learning course.
📊 Result
Public Score: 15,577 MAE (Mean Absolute Error)
🛠️ Tech Stack

Python
Pandas
Scikit-learn (Pipelines, ColumnTransformer, SimpleImputer, OneHotEncoder)
XGBoost
Kaggle Notebooks

🔍 Approach
1. Data Preprocessing

Separated numerical and categorical columns
Handled missing values:

Numerical → filled with median using SimpleImputer
Categorical → filled with constant 'Missing' using SimpleImputer


Encoded categorical features using OneHotEncoder(handle_unknown='ignore')

2. Pipeline Architecture
Built a full sklearn Pipeline with ColumnTransformer for clean, scalable preprocessing:
ColumnTransformer
├── Categorical: SimpleImputer → OneHotEncoder
└── Numerical:  SimpleImputer
3. Model

Used XGBRegressor from XGBoost
learning_rate=0.05, n_estimators=250, random_state=0

📁 Files
FileDescriptionhouse-price-prediction.ipynbMain notebook with full codes ubmission.csvFinal predictions submitted to Kaggle
🚀 What I Learned

Building end-to-end Sklearn Pipelines for clean preprocessing
Using ColumnTransformer to handle numerical and categorical columns separately
XGBoost for regression problems
Why pipelines prevent data leakage better than manual preprocessing
Difference between MAE (regression) and Accuracy (classification)

📈 Upgrade from Previous Project (Titanic)
TitanicHouse PricesModelRandom Forest ClassifierXGBoost RegressorPreprocessingManual fillnaFull PipelineEncodingget_dummiesOneHotEncoderProblem TypeClassificationRegression
🔗 Previous Project
Titanic Survival Prediction
📈 Future Improvements

 Use full training data for final submission (without validation split)
 Hyperparameter tuning with cross-validation
 Feature engineering on key columns
