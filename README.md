# Wine Quality Prediction using Machine Learning

Overview
This project aims to predict the quality of wine based on physicochemical properties, using various machine learning techniques. By leveraging the Wine Quality dataset, we explore models including Logistic Regression, Decision Trees, and Support Vector Machines (SVM) to accurately classify wine quality, providing a framework for enhanced decision-making in the wine industry. Through a structured pipeline—data cleaning, exploratory data analysis, feature engineering, model training, and hyperparameter tuning—we achieved notable results that showcase the potential of machine learning for quality assessment.

1.Table of Contents.
2.Dataset.
3.Project Structure.
4.Installation.
5.Data Preprocessing.
6.Exploratory Data Analysis.
7.Model Training and Evaluation.
8.Results.
9.Conclusion.
10.Google Colab Notebook.
11.Contributors.
12.Dataset.
The dataset used for this project is the Wine Quality dataset, which is publicly available from the UCI Machine Learning Repository. It contains various physicochemical properties of red and white wines, including:

Fixed Acidity
Volatile Acidity
Citric Acid
Residual Sugar
Chlorides
Free Sulfur Dioxide
Total Sulfur Dioxide
Density
pH
Sulphates
Alcohol
The target variable is the quality rating of wine, which is an integer score between 0 and 10.

Data Preprocessing
Data preprocessing steps include:

Handling Missing Values: Missing values were imputed or handled as necessary.
Outlier Detection and Handling: Identified and processed outliers using Z-score and IQR methods.
Normalization: All features were normalized to ensure consistent scaling.
Encoding Categorical Variables: Applied one-hot encoding for categorical features to convert them into numerical format.
Preprocessing scripts can be found in src/data_preprocessing.py.

Exploratory Data Analysis
The exploratory data analysis (EDA) phase helped us understand key features influencing wine quality. Visualizations include:

Correlation Matrix: Highlights relationships between features.
Distribution Analysis: Histograms and box plots show distributions of variables.
Feature Importance: Decision Tree and SVM feature importance analyses highlight which physicochemical properties impact quality predictions most.
All EDA work is documented in the notebooks/EDA.ipynb notebook.

Model Training and Evaluation
We trained three machine learning models and evaluated their performance:

Logistic Regression: Trained to provide a baseline and interpret model performance with fewer computational resources.
Decision Tree: Chosen for its high interpretability and strong performance.
Support Vector Machine (SVM): Offers robust results but is computationally intensive.
Each model’s hyperparameters were tuned through grid search, and models were evaluated on accuracy, precision, recall, and F1-score. Training and evaluation scripts are located in src/model_training.py and src/evaluation.py.

Results
Our model results were as follows:

Decision Tree: Highest accuracy of 85% with a balanced F1-score of 0.83.
Support Vector Machine: Accuracy of 82%, F1-score of 0.80.
Logistic Regression: Accuracy of 80%, F1-score of 0.76.
For more detailed performance metrics, please refer to the Results section in results/.

Confusion Matrix
The confusion matrix for the Decision Tree model demonstrated a high rate of correct predictions, underscoring its effectiveness in classifying wine quality accurately.

Conclusion
This project demonstrates the potential of machine learning in predicting wine quality based on physicochemical properties. The Decision Tree model emerged as the most effective, though each model provided valuable insights and considerations for practical applications. The findings suggest that machine learning can support quality assessments in the wine industry, balancing accuracy with model interpretability and resource demands.
