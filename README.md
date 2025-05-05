
# Loan Approval Prediction (Neural Network Project)

## 📌 Problem Description

The main objective of this project is to **predict whether a person qualifies for a loan or not**, based on various personal and financial attributes.  
The model aims to assist in making informed decisions for loan approvals by predicting `loan_status` (approved or not approved).

## 🧠 Approach

The project followed several steps to design, train, and optimize the neural network model:

- **Data preprocessing**: Removing unnecessary elements from the dataset.
- **Model building**: Initially with Backpropagation and Forward Propagation algorithms.
- **Model optimization** using:
  - Adjusting the number of layers.
  - Tuning initial weights.
  - Changing learning rates.
  - Applying regularization and dropout to prevent overfitting.

### Model Iteration Summary

| Model Version | Layers | Accuracy | Notes |
|---------------|--------|----------|-------|
| Initial Model | 1      | 0.9322   | Simple architecture, gradual loss reduction |
| Improved Model | 2      | 0.9450   | Better accuracy and lower initial loss |
| Final Model (With best hyperparameters) | N/A | 0.97 | Learning Rate = 0.0001 |

### Overfitting Prevention

- **Regularization** and **Dropout layers** (Dropout = 0.2 and 0.3) were introduced:
  - Dropout = 0.2 → Accuracy 0.942
  - Dropout = 0.3 → Accuracy 0.93

### Final Recommendation

- **Best Accuracy** → Learning Rate `0.0001` (Accuracy = 0.97)
- **Best Loss Minimization** → Learning Rate `0.01`
- **Balanced Model** → Regularization with Dropout `0.3`

## 📊 Dataset Details

| Feature | Description |
|---------|-------------|
| person_age | Person's age |
| person_income | Annual income |
| person_home_ownership | Home ownership status |
| person_emp_length | Years of employment |
| loan_intent | Purpose of the loan |
| loan_grade | Loan grade |
| loan_amnt | Loan amount |
| loan_int_rate | Loan interest rate |
| loan_percent_income | Loan amount as a percentage of income |
| cb_person_default_on_file | Previous bankruptcy record |
| cb_person_cred_hist_length | Credit history length |
| loan_status | Loan status (0 = No Default, 1 = Default) |

## 🎯 Competition Rules

- No cheating or data leakage allowed.
- Only ethical and legal methods used.
- Training and test data provided.
- Objective: Build a model that predicts loan approval status accurately.

## 👨‍💻 Team Members

- **Walid Tamer** (22100805)
- **Rawan Ayman Adli** (21100867)
- **Shams Abd Elhalim** (22101040)
- **Sara Samir Nasr** (22101068)

## 📈 Project Results

Through careful tuning and improvements:
- **Highest Achieved Accuracy:** 0.97
- **Best Model Parameters:** Learning Rate `0.0001`, regularization techniques applied to avoid overfitting.
