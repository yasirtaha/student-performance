# Student Performance Regression
Overview
This project focuses on predicting student exam scores based on various features related to their study habits, attendance, and personal characteristics. The dataset is structured for regression analysis, where the goal is to accurately forecast a continuous variable, Exam_Score, based on input features.

Dataset
The dataset consists of the following features:

Hours_Studied: Number of hours studied by the student.
Attendance: Attendance percentage of the student.
Parental_Involvement: Involvement level of parents in the student's education (Low, Medium, High).
Access_to_Resources: Access to study resources (Low, Medium, High).
Extracurricular_Activities: Whether the student participates in extracurricular activities (Yes, No).
Sleep_Hours: Average number of sleep hours per day.
Previous_Scores: Scores from previous exams.
Motivation_Level: The student's level of motivation (Low, Medium, High).
Internet_Access: Whether the student has access to the internet (Yes, No).
Tutoring_Sessions: Number of tutoring sessions attended.
Family_Income: Family income level (Low, Medium, High).
Teacher_Quality: Perception of the teacher's quality (Low, Medium, High).
School_Type: Type of school attended (Public, Private).
Peer_Influence: The level of peer influence on the student (Negative, Neutral, Positive).
Physical_Activity: Number of hours spent on physical activities per week.
Learning_Disabilities: Whether the student has learning disabilities (Yes, No).
Parental_Education_Level: Education level of the parents (High School, College, Postgraduate).
Distance_from_Home: Distance from the student's home to school (Near, Moderate, Far).
Gender: Gender of the student (Male, Female).
Exam_Score: The score obtained by the student in the exam (Target variable for regression).
Project Workflow
1. Data Preprocessing
Handled missing values: Cleaned up null values through imputation and row removal.
Applied one-hot encoding for nominal categorical variables and label encoding for ordinal variables.
Engineered the Grade column, which categorizes students based on exam scores, for exploratory purposes (not used in the regression model).
2. Exploratory Data Analysis
Descriptive statistics and visualizations were performed to understand feature distributions and their relationships with the target variable, Exam_Score.
Examined correlations between the features and the exam scores to identify key predictors.
3. Feature Engineering
Selected features for regression modeling, performing necessary encoding and scaling.
4. Model Building and Evaluation
The following regression models were implemented to predict student exam scores:

Linear Regression
Random Forest Regressor
Support Vector Regressor (SVR)
The models were evaluated using the following metrics:

Mean Squared Error (MSE)
Root Mean Squared Error (RMSE)
Mean Absolute Error (MAE)
R-squared (R²)
5. Hyperparameter Tuning
GridSearchCV was used to tune hyperparameters for optimal performance of the Random Forest Regressor and SVR.
Results
The best-performing models were compared based on error metrics, and feature importance analysis was conducted for the Random Forest model. Key takeaways include:

Significant predictors of exam scores, such as Hours Studied and Previous Scores.
Performance comparison of linear and non-linear regression models.
Improvements achieved through hyperparameter tuning.
Installation
To run the project locally, follow these steps:

Clone the repository:

bash
Copy code
git clone https://github.com/your-username/student-performance-regression.git
Install the required dependencies:

bash
Copy code
pip install -r requirements.txt
Usage
Open Group11.ipynb in Jupyter Notebook or JupyterLab.
Run the cells sequentially to:
Preprocess the dataset.
Train regression models.
Evaluate model performance and make predictions.
Contributing
If you'd like to contribute:

Fork the repository.
Create a new feature branch (git checkout -b feature-branch).
Commit your changes (git commit -m 'Add feature').
Push to the branch (git push origin feature-branch).
Open a pull request.


Acknowledgments
Dataset source: [Mention the source]
Special thanks to collaborators and instructors.
