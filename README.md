# 🍇 Wine Quality Prediction Project

## 📝 Overview
This project implements and compares various regression models to predict the quality of red and white wines based on their chemical properties. It uses the combined datasets `winequality-red.csv` and `winequality-white.csv`.  

The results indicate that the **Random Forest Regressor** provides the best predictive performance, achieving higher R² and lower Mean Squared Error (MSE) compared to other models.


## 🛠️ Requirements
To run the Jupyter Notebook, you need the following Python libraries:

pip install pandas scikit-learn

## ⚙️ Workflow

Data Loading: Load red (winequality-red.csv) and white (winequality-white.csv) wine datasets and combine them.

Data Preprocessing: Concatenate both DataFrames into a single wine_data object and check for missing values (NaN).

Train/Test Split: Separate features (X) and target (y, the quality column), then split into 80:20 training and testing sets (random_state=42).

Model Training & Evaluation: Train three regression models and evaluate them using Mean Squared Error (MSE) and R² Score.

## 📊 Model Evaluation Results
| Model                   | MSE (Mean Squared Error) | R² Score |
| ----------------------- | ------------------------ | -------- |
| Decision Tree Regressor | 0.653                    | 0.086    |
| Linear Regression       | 0.477                    | 0.333    |
| Random Forest Regressor | 0.318                    | 0.555    |


The Random Forest Regressor shows the best predictive performance with the lowest MSE and highest R² score.

### 🚀 Next Steps

Hyperparameter Tuning: Use GridSearchCV or RandomizedSearchCV on the Random Forest Regressor to maximize performance.

Feature Importance Analysis: Identify which chemical properties most influence wine quality.

Classification Approach: Convert continuous quality scores into discrete classes (e.g., "low," "medium," "high") and explore classification models.
