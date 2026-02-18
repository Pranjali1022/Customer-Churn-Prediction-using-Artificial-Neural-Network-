# Customer Churn Prediction using Artificial Neural Network (ANN)

## 📌 Project Overview

This project predicts whether a bank customer is likely to churn (leave the bank) using a deep learning model built with TensorFlow/Keras.
The solution includes:

* Data preprocessing pipeline (encoding + scaling)
* Artificial Neural Network model
* Model persistence using `.h5` and `.pkl` files
* Streamlit web application for real-time prediction

The system takes customer attributes as input and outputs the probability of churn.

---

## 🎯 Objectives

* Build a supervised machine learning model to predict customer churn
* Apply feature engineering and preprocessing techniques
* Deploy the trained ANN model via a user-friendly web interface
* Demonstrate an end-to-end ML workflow from training to deployment

---

## 📂 Project Structure

```
├── app.py                     # Streamlit web app for prediction
├── model.h5                   # Trained ANN model
├── scaler.pkl                 # StandardScaler object
├── onehot_encoder_geo.pkl     # OneHotEncoder for geography
├── label_encoder_gender.pkl   # LabelEncoder for gender
├── Prediction.ipynb           # Notebook for model inference/testing
├── requirements.txt           # Required Python packages
└── README.md                  # Project documentation
```

---

## 🧠 Model Details

* Model type: Artificial Neural Network (ANN)
* Framework: TensorFlow / Keras
* Task: Binary Classification
* Target variable: Customer Churn 

### Input Features Used

* Credit Score
* Age
* Gender
* Tenure
* Balance
* Number of Products
* Credit Card Ownership
* Active Membership
* Estimated Salary
* Geography (One-Hot Encoded)

---

## ⚙️ Preprocessing Pipeline

1. **Label Encoding**

   * Gender converted into numeric labels

2. **One-Hot Encoding**

   * Geography converted into dummy variables

3. **Feature Scaling**

   * StandardScaler applied to normalize inputs

The same encoders and scaler used during training are saved and reused for prediction.

---

## 🖥️ Web App Features

* Interactive form for customer inputs
* Automatic preprocessing pipeline
* Real-time ANN prediction
* Clean UI powered by Streamlit

---

## 📊 Example Output

The model returns:

* Probability of churn
* Binary prediction (Likely to churn / Not likely to Churn)

---

## 🔮 Future Improvements

* Add model explainability 
* Include probability visualization
* Improve model using hyperparameter tuning
* Deploy on cloud (Streamlit Cloud / AWS )
* Add API endpoint for integration

---

## 👩‍💻 Author

**Pranjali Patil**
M.Tech, IIT Kharagpur

---

## 📜 License

This project is for academic and learning purposes.
