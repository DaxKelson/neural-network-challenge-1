# Student Loan Repayment Classification with Neural Networks

## Overview

This project uses a deep learning approach to classify student loan repayment success based on various student financial and academic features. The objective is to build, train, evaluate, and deploy a neural network model using TensorFlow and Keras to predict the likelihood of a student's successful loan repayment.

---

## Technologies

- Python 3.10+
- Pandas
- TensorFlow/Keras
- scikit-learn
- Google Colab

---

## Data

The dataset used for this project was provided via the following URL:
https://static.bc-edx.com/ai/ail-v-1-0/m18/lms/datasets/student-loans.csv
The dataset includes the following columns:
- `loan_amount`
- `interest_rate`
- `loan_term`
- `monthly_payment`
- `gpa`
- `credit_hours`
- `age`
- `credit_ranking` (Target)

---

## Methodology

1. **Data Preparation**
   - Loaded the dataset and reviewed data types.
   - Defined the feature matrix `X` and target vector `y`.
   - Split the data into training and testing sets.
   - Applied standard scaling to the feature data.

2. **Model Creation and Training**
   - Built a Sequential deep learning model with two hidden layers using ReLU activation.
   - Compiled the model using `binary_crossentropy` and the Adam optimizer.
   - Trained the model over 50 epochs on the training data.

3. **Model Evaluation**
   - Evaluated the model on test data using loss and accuracy metrics.
   - Used predictions to generate a classification report.

4. **Model Deployment**
   - Saved the trained model as a `.keras` file.
   - Reloaded the model and used it to predict repayment success on test data.

---

## Results

- Achieved 0.7600 accuracy on the test set.

---

## Challenges

- Ensuring that feature scaling did not leak information from test data.
- Designing a balanced architecture to avoid overfitting or underfitting.

---

## Ethical Considerations

Two major challenges identified for building a real-world recommendation system for student loans:
1. **Fairness & Bias**: Preventing algorithmic discrimination against specific student groups based on socioeconomic background or academic history.
2. **Privacy & Data Collection**: Safeguarding sensitive personal and financial data used to inform loan recommendations.

---

## Future Work

- Explore regularization techniques to further improve model generalization.
- Implement explainable AI tools to interpret predictions and build trust.
- Integrate fairness evaluation metrics and bias mitigation strategies.

---

## Author

Dax Kelson
5/16/2025
