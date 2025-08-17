🩺 Diabetes Prediction using Support Vector Machine (SVM)
📌 Problem Statement
Can we predict whether a person is diabetic or non-diabetic based on their medical records such as glucose level, BMI, age, and other health factors?

📌 Solution Statement
We use a Support Vector Machine (SVM) classifier with a linear kernel to analyze medical data and predict diabetes status. The model is trained on the PIMA Indian Diabetes dataset, performs data standardization, and provides predictions with good accuracy.

🗂 Dataset
The dataset diabetes.csv includes the following features:
Pregnancies → Number of pregnancies
Glucose → Plasma glucose concentration
BloodPressure → Diastolic blood pressure (mm Hg)
SkinThickness → Triceps skinfold thickness (mm)
Insulin → Serum insulin (mu U/ml)
BMI → Body Mass Index (weight in kg / height in m²)
DiabetesPedigreeFunction → Diabetes heredity function score
Age → Age of the person
Outcome → Target variable (0 = Non-diabetic, 1 = Diabetic)

⚙️ Project Workflow
Data Collection & Preprocessing
Loads the dataset and converts column names to lowercase
Analyzes dataset shape, summary statistics, and distribution of target variable (Outcome)
Feature Standardization
Standardizes features using StandardScaler to normalize values
Train-Test Split
Splits dataset into 80% training and 20% testing sets
Stratified sampling ensures equal representation of diabetic/non-diabetic
Model Training (SVM Classifier)
Trains an SVM with linear kernel on training data
Fits decision boundary to classify diabetic vs non-diabetic

Model Evaluation
Evaluates using Accuracy Score on training and testing sets
Accuracy > 75% is considered good performance
User Input Prediction
Takes user medical details as input (Pregnancies, Glucose, Blood Pressure, BMI, etc.)
Standardizes input data and predicts diabetic or non-diabetic outcome

Visualizations
Scatter plots for relationships between health features and diabetes outcome
Grid of plots for all features vs outcome to analyze patterns

📊 Example Results
Training Accuracy: ~78–80%
Testing Accuracy: ~76–78%
User Input Example:
Pregnancies: 4
Glucose: 110
BloodPressure: 92
...
Prediction → The person is diabetic

⚙️ Technologies & Libraries Used
Python
Pandas – Data analysis
NumPy – Mathematical computations
Matplotlib – Visualization
Scikit-Learn – StandardScaler, Train-Test Split, SVM Classifier, Accuracy Metrics

💡 Highlights of This Project
Implements SVM classifier for binary classification
Provides interactive user input prediction
Includes data standardization for better model accuracy
Visualizes feature relationships with outcome

Beginner-friendly healthcare ML project that can be extended into a web app (Streamlit/Flask
