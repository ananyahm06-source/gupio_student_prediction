# Student Academic Outcome Prediction

## Project Description

This project predicts the academic outcome of students using Machine Learning.

The target classes are:
- Dropout
- Enrolled
- Graduate

The model uses information that is available at the time of student enrollment.

## Dataset

The dataset is the UCI Predict Students' Dropout and Academic Success dataset.

The supplied assessment dataset file is `data.csv`.

Dataset contains 4424 student records.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## Data Preprocessing

The dataset was inspected for:
- Missing values
- Duplicate records
- Data types
- Target class distribution

The 12 first and second semester variables were removed because they are not available at enrollment and could cause data leakage.

The data was divided into:
- 80% Training data
- 20% Testing data

Stratified splitting was used to maintain the target class distribution.

## Machine Learning Models

Two classification models were trained:

1. Logistic Regression
2. Random Forest Classifier

## Evaluation

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Macro F1-score
- Confusion Matrix

The final model was selected based on Macro F1-score.

## Sample Prediction

The final model was used to predict academic outcomes for sample student records from the test dataset.

## Feature Importance

Important predictive features were identified from the final model.

Feature importance indicates which features are useful for prediction. It does not prove that a feature causes the academic outcome.

## Limitations

- The model predicts academic outcomes based on available enrollment-time information.
- Prediction does not establish causal relationships.
- Model performance depends on the supplied dataset.
- The model should not be treated as a guaranteed prediction of an individual student's future.

## How to Run

1. Install Python.
2. Install the required libraries using:

   pip install -r requirements.txt

3. Open the Jupyter Notebook:

   notebooks/student_prediction.ipynb

4. Run the notebook from beginning to end.