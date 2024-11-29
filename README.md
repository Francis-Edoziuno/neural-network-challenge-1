# neural-network-challenge-1
# Student Loan Risk with Deep Learning
This repository demonstrates a workflow to predict student loan repayment success using deep learning techniques. The process involves data preprocessing, model development, evaluation, and predictions. The results include a trained neural network model that predicts loan repayment success based on historical data.

# Features
Data Preprocessing: Reads, reviews, and preprocesses a dataset containing student loan-related features.
Deep Neural Network: Implements a TensorFlow-based Sequential model with two hidden layers to predict loan repayment success.
Model Evaluation: Evaluates the trained model on test data and generates a classification report.
Model Persistence: Exports the trained model for future use.
Prediction: Reloads the saved model and predicts repayment success.

# Workflow
1. Data Preparation
Input Data: student-loans.csv containing features such as payment history, GPA, financial aid scores, and credit ranking.
Target Variable: credit_ranking (0 or 1), indicating loan repayment success.
Preprocessed features and target variable are split into training and test datasets, and standardized using StandardScaler.

2. Neural Network Model
Architecture:
Input Layer: 11 features
Hidden Layer 1: 6 neurons with ReLU activation
Hidden Layer 2: 3 neurons with ReLU activation
Output Layer: 1 neuron with linear activation
Compilation: Uses mean_squared_error as the loss function, adam optimizer, and evaluates on mse.
Training: Trains over 50 epochs on the training data.

3. Model Evaluation and Predictions
Evaluates the model on test data, measuring loss and mean squared error.
Makes predictions on test data, rounding results to binary values (0 or 1).
Generates a classification report to assess precision, recall, and F1-score.

4. Model Persistence
Saves the trained model as student_loans.keras for reuse.
Reloads the saved model to make predictions.
Results
Model Performance: Classification report indicates approximately 76% accuracy, precision, recall, and F1-score.
Saved Model: Trained model is exported and available for further predictions.


# Recommendations for Improvement
Data for Recommendation System
To build a recommendation system for student loans:

# Data Requirements:
Academic profile (GPA, major, expected graduation date)
Financial information (income, savings, loan preferences)
Educational costs (tuition, living expenses)
Loan attributes (interest rates, repayment terms, lender details)

# Filtering Method:

Context-based filtering: This method matches students with loans based on their specific circumstances (e.g., financial needs, academic profile) rather than comparing with peers.

# Challenges:

Data Privacy: Protecting sensitive financial and personal information.
Bias in Recommendations: Avoiding over-recommendation of loans with unfavorable terms or from specific lenders.

