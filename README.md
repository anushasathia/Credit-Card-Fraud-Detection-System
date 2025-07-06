# 💳 Credit Card Fraud Detection System

## 🚀 Overview

This project presents a **streamlined Credit Card Fraud Detection System** that leverages machine learning to detect and flag potentially fraudulent credit card transactions.

The application combines a **Streamlit-powered web interface** with a Python backend to deliver real-time insights, enabling security teams and analysts to make swift, informed decisions. It effectively learns transaction behavior and detects anomalies, even within imbalanced datasets.

---

## 🌟 Core Features

- 🔐 **User Login System**: Secure authentication for users, with admin-level privileges for model and user management.
- 📁 **CSV Upload**: Seamless data upload to feed the fraud detection engine.
- 🧠 **Fraud Analysis**: Predicts whether a transaction is `legitimate` or `fraudulent` using a pre-trained Logistic Regression model.
- 📈 **Prediction Output & Metrics**:
  - Highlights suspicious entries
  - Provides evaluation metrics (Accuracy, Precision, Recall, F1-Score)
  - Displays a Confusion Matrix for transparency
- ⚡ **Live Feedback**: Shows total transactions, fraud count, and model confidence instantly after upload.
- 🛡 **Admin Controls**: Allows admins to upload and manage models and scalers, with version control support.
- 🎨 **User Preferences**: Customize experience with light/dark mode and alert settings.
- 🧹 **Preprocessing Pipeline**: Automatically scales and prepares transaction data for analysis.
- ⚖️ **Class Imbalance Handling**: Uses undersampling (via `imblearn`) to balance fraud vs. legitimate cases during training.

---

## 📸 Screenshots

### 🔐 Login Interface  
Secure login system for both regular users and administrators.  
![image alt](https://github.com/rohanpahari3/Credit-Card-Fraud-Detection/blob/ef1bb7276e804183c87e9ca668568de109f31de2/Screenshot%202025-07-06%20194110.png)

### ✅ Legitimate Transaction Output  
Displays transactions that are predicted to be safe.  
![image alt](https://github.com/rohanpahari3/Credit-Card-Fraud-Detection/blob/a29997a3592e5d1d5766eedc745b8bc2be1fe01c/Screenshot%202025-07-06%20194215.png)

### 🚨 Fraudulent Transaction Output  
Highlights potentially fraudulent activities.  
![image alt](https://github.com/rohanpahari3/Credit-Card-Fraud-Detection/blob/a29997a3592e5d1d5766eedc745b8bc2be1fe01c/Screenshot%202025-07-06%20194245.png)

### 🧮 Confusion Matrix  
Visual representation of the model’s classification performance.  
![image alt](https://github.com/rohanpahari3/Credit-Card-Fraud-Detection/blob/a29997a3592e5d1d5766eedc745b8bc2be1fe01c/Screenshot%202025-07-06%20194309.png)

---

## 🏗 Architecture

The system is based on a **client-server model**, separating UI and backend responsibilities for modularity and performance.

- **Frontend**: Built with **Streamlit** to offer a clean and dynamic user interface.
- **Backend**: Developed in **Python**, it:
  - Processes uploaded files
  - Executes the Logistic Regression model
  - Outputs results and performance metrics
- **Machine Learning Core**: Implements scikit-learn to train and deploy fraud detection models.

---

## 🧰 Tech Stack

| Category              | Tools & Libraries                                |
|-----------------------|--------------------------------------------------|
| Language              | Python                                           |
| Framework             | Streamlit                                       |
| Data Handling         | pandas, numpy                                   |
| ML Libraries          | scikit-learn, imbalanced-learn (`imblearn`)     |
| Visualization         | matplotlib, seaborn                             |
| Versioning            | Git, GitHub                                     |
| Package Management    | pip                                             |

---

## ▶️ How to Run

To start the app locally, run:

```bash
streamlit run app.py
