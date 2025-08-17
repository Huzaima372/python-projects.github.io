❤️ Heart Disease Prediction using Logistic Regression

📌 Problem Statement

Heart disease is one of the leading causes of death worldwide. Can we build a machine learning model that predicts whether a person is at risk of heart disease based on medical attributes such as age, cholesterol, blood pressure, and more?


📌 Solution Statement

We apply a Logistic Regression model trained on patient health records to classify whether a person has heart disease (1) or does not have heart disease (0). The dataset is preprocessed, scaled, and evaluated for accuracy.


🗂 Dataset

The dataset heart_disease_data.csv contains patient health records with features like:

Age → Age of the patient

Sex → Gender (1 = Male, 0 = Female)

Chest Pain Type (cp) → Type of chest pain

Resting Blood Pressure (trestbps) → Blood pressure (mm Hg)

Cholesterol (chol) → Serum cholesterol (mg/dl)

Fasting Blood Sugar (fbs) → (1 = true if >120 mg/dl, else 0)

Resting ECG (restecg) → Resting electrocardiographic results

Max Heart Rate Achieved (thalach)

Exercise Induced Angina (exang)

ST Depression (oldpeak)

Slope of ST Segment (slope)

Number of Major Vessels (ca)

Thalassemia (thal)

Target (outcome) → (1 = has heart disease, 0 = no heart disease)


⚙️ Project Workflow

Data Loading & Preprocessing

Load dataset with Pandas

Check for missing values and statistical summaries

Scale features using StandardScaler

Train-Test Split

Dataset is split into training (90%) and testing (10%) sets

Stratified sampling ensures balanced class distribution

Model Training

Logistic Regression classifier trained on scaled data

Model Evaluation

Accuracy score on both training and test sets

Additional evaluation metrics:

Mean Absolute Error (MAE)

Mean Squared Error (MSE)

R² Score

User Input Prediction

Interactive input for medical attributes

Model predicts whether the person is at risk of heart disease or not

Visualization

Scatter plot of predictions vs actual outcomes

Histogram showing distribution of target variable


📊 Example Results

Training Accuracy: ~85–90%

Testing Accuracy: ~80–85%

Example Input:

Age: 57
Sex: 1
Chest Pain Type: 0
...
Prediction → The person has a heart disease


⚙️ Technologies & Libraries Used

Python

Pandas – Data handling

NumPy – Numerical operations

Matplotlib – Data visualization

Scikit-Learn – StandardScaler, Logistic Regression, evaluation metrics


💡 Highlights of This Project

Predicts heart disease risk based on patient medical attributes

Uses Logistic Regression for classification

Includes user input-based prediction

Provides accuracy and error metrics for evaluation

Beginner-friendly healthcare ML project

Can be extended into a web app (Flask/Streamlit) for real-time prediction
