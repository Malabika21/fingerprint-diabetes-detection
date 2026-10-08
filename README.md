# Fingerprint Diabetes Detection

An AI-powered diabetes risk prediction web application built with Python and Flask that uses fingerprint image analysis and machine learning to predict diabetes risk based on fingerprint features and patient health parameters such as age, BMI, and family history.

🚀 Live Demo  
https://fingerprint-diabetes-detection.onrender.com

## 📌 Project Overview

Fingerprint Diabetes Detection combines image processing and machine learning to estimate diabetes risk from fingerprint patterns along with clinical and lifestyle parameters.

The web application provides an intuitive interface where users can upload fingerprint images, enter relevant patient information, and receive a diabetes risk prediction.

### Supported Diagnostics

- 🖐️ Fingerprint Pattern Analysis
- 🩺 Diabetes Risk Prediction
- 📊 Clinical Parameter-Based Risk Assessment
- 📈 Machine Learning-Based Classification

## ✨ Features

- 📊 Interactive Web Interface built with Flask and Jinja2 templates
- 🖐️ Fingerprint image processing using OpenCV and PIL
- 🤖 Machine Learning-based diabetes risk classification
- 📋 Patient parameter analysis using Age, BMI, and Family History
- ⚡ Automated fingerprint feature extraction
- 🔄 Pre-trained model and label encoders for real-time prediction
- 💾 SQLite database integration for user/application data
- 🔐 User authentication and session management
- 🌐 Cloud deployment optimized for Render Web Services

## 🧠 Machine Learning Architecture

The core prediction system combines fingerprint-derived features with patient health parameters to classify diabetes risk.

### Features and Data Pipeline

- Fingerprint image preprocessing and feature extraction
- Fingerprint pattern classification
- Age and BMI-based clinical parameters
- Family history information
- Pre-trained machine learning model (`diabetes_model.pkl`)
- Label encoders for categorical features

The trained model and encoders are stored in the `model/` directory and loaded by the Flask application during runtime.

## 📊 Prediction Logic

The prediction pipeline processes the user's fingerprint and health information before passing the extracted features to the trained machine learning model.

The pipeline includes:

- Fingerprint image preprocessing using OpenCV/PIL
- Extraction and processing of relevant fingerprint features
- Encoding of categorical parameters using pre-trained label encoders
- Integration of fingerprint features with patient parameters such as age, BMI, and family history
- The trained machine learning model generates a diabetes risk prediction
- The prediction is presented through the web interface

## 🛠️ Technologies Used

- Python 3.10
- Flask
- Gunicorn
- Scikit-Learn
- Pandas
- NumPy
- OpenCV
- Pillow
- Joblib
- SQLite3
- HTML5 / CSS3
- Jinja2
- Render

## 📂 Project Structure

```text
fingerprint-diabetes-detection/
│
├── model/
│   ├── diabetes_model.pkl
│   ├── le_diabetes_risk.pkl
│   ├── le_family_history.pkl
│   └── le_fingerprint.pkl
│
├── static/
├── templates/
├── Test Images/
├── uploads/
├── notebooks/
│
├── app.py
├── train.py
├── fingerprint_diabetes_dataset.csv
├── requirements.txt
├── .gitignore
├── users.db
└── README.md
