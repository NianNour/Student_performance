# Student_performance
# 🎓 Student Performance Prediction using Linear Regression

This project implements a simple linear regression model to predict a student's **Performance Index** based on various academic and lifestyle factors using **scikit-learn**'s `SGDRegressor`.

## 📊 Features Used

The following features from the dataset were used as input variables:

- `Hours Studied`
- `Previous Scores`
- `Extracurricular Activities`
- `Sleep Hours`
- `Sample Question Papers Practiced`

The target variable is:

- `Performance Index`

---

## 🧠 Goal

The goal is to build and evaluate a regression model that can predict a student's performance using input features. The project includes:

- Visualizing feature-target relationships
- Normalizing features using z-score
- Training a linear regression model with stochastic gradient descent (SGD)
- Evaluating the model on a test set
- Predicting new examples

---

## 🛠️ Technologies & Libraries

- Python 3
- NumPy
- Pandas
- Matplotlib
- scikit-learn

---

## 🗂️ Workflow

1. **Load the dataset**  
   The first 2000 rows of `Student_Performance.csv` are used.

2. **Train-test split**  
   The dataset is split into:
   - 1300 samples for training
   - 700 samples for testing

3. **Visualization**  
   Scatter plots are created to show the relationship between each feature and the performance index.

4. **Normalization**  
   Features are normalized using `StandardScaler` to improve model training.

5. **Model Training**  
   A linear regression model is trained using `SGDRegressor`.

6. **Prediction & Plotting**  
   Predictions on the training set are compared visually against actual values.

7. **Model Evaluation**  
   The model is evaluated on the test set using:
   - Mean Squared Error (MSE)
   - R² Score

8. **New Prediction**  
   The model predicts the performance of a new student with manually entered values.

---

## 📈 Sample Prediction

```python
# New student data:
[Hours Studied=8, Previous Scores=80, Extracurricular Activities=1, Sleep Hours=9, Sample Papers=5]
→ Predicted Performance Index: 76.91
