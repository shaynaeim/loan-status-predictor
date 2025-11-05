# 💰 LendingClub Loan Repayment Prediction

A **deep learning model** for predicting loan repayment risk using the **LendingClub dataset**.  
This project uses the **Keras API** with **TensorFlow** to build and train a binary classification model that determines whether a borrower is likely to **repay** or **default** on a loan.

---

## 📘 Project Overview

The LendingClub dataset contains borrower details such as income, credit history, and loan purpose.  
Our goal is to develop a model that can assess loan repayment risk — helping lenders make informed credit decisions.

This project demonstrates:
- How to prepare real-world financial data for deep learning.
- How to design and train a **binary classification neural network**.
- How to evaluate model performance using appropriate metrics.

---

## 🧠 Key Objectives

- Perform **data cleaning** and **feature engineering** on financial data.  
- Build and train a **neural network** using Keras (TensorFlow backend).  
- Use **binary cross-entropy loss** and metrics such as **accuracy**, **precision**, and **recall**.  
- Visualize training performance and evaluate the model on unseen data.

---

## 🧩 Technologies Used

- **Python 3.10+**  
- **TensorFlow / Keras**  
- **Pandas**  
- **NumPy**  
- **Matplotlib**  
- **Seaborn**  
- **scikit-learn**

---

## 🚀 Project Workflow

1. **Data Exploration (EDA)**
   - Load and inspect LendingClub data.
   - Handle missing values and categorical features.

2. **Data Preprocessing**
   - Feature scaling and encoding.
   - Train/test data split.

3. **Model Building**
   - Sequential deep neural network using Keras.
   - Dense layers with ReLU activation and dropout regularization.

4. **Model Training**
   - Compile with `binary_crossentropy` loss and the `adam` optimizer.
   - Train and validate the model using training data.

5. **Evaluation**
   - Generate accuracy, confusion matrix, and classification report.
   - Plot loss and accuracy curves.

---


model.compile(optimizer='adam', loss='binary_crossentropy', metrics=['accuracy'])
history = model.fit(X_train, y_train, validation_data=(X_test, y_test), epochs=25, batch_size=64)
