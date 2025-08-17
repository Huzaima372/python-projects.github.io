Pakistan Students Marks Prediction using Linear Regression

📌 Problem Statement
Can we check if study hours per week and midterm scores have an impact on a student’s final score?

📌 Solution Statement
We apply Linear Regression to learn the relationship between study hours, midterm performance, and final scores.
The trained model is then used to predict final exam marks.

🗂 Dataset
The dataset student_dataset_pakistan_updated.csv contains the following columns:
study_hour_per_week → Number of hours a student studies per week
midterm_score → Marks obtained in midterm
final_score → Marks obtained in the final exam (target variable)

⚙️ Project Workflow
Dataset Loading & Preprocessing
Loads dataset into a Pandas DataFrame
Converts column names to lowercase for consistency
Checks for missing values
Exploratory Data Analysis (EDA)

Distribution of final_score visualized using a histogram
Scatter plot of study hours vs marks
Model Training (Linear Regression)
Model 1: Uses only study_hour_per_week as input feature
Model 2: Uses both study_hour_per_week and midterm_score as input features
Fits a Linear Regression model using Scikit-Learn

Model Evaluation
Metrics used:
Mean Absolute Error (MAE)
Mean Squared Error (MSE)
Root Mean Squared Error (RMSE)
R² Score (goodness of fit)
Prints model parameters (intercept and coefficients)

Visualizations
Histogram of student final scores
Scatter plots showing actual vs predicted relationships
Line plots for predicted final scores vs study hours & midterm marks
Prediction with User Input
Accepts study hours input from the user
Predicts expected final score using the trained model

📊 Example Results
Model intercept and coefficients show how study hours and midterm marks affect final exam marks.
Evaluation metrics indicate prediction accuracy:
MAE ≈ (small value → better accuracy)
R² Score close to 1 → good fit

⚙️ Technologies & Libraries Used
Python
Pandas – Data handling
NumPy – Mathematical computations
Matplotlib – Data visualization
Scikit-Learn – Linear Regression & evaluation metrics
