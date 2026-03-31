# Diabetes Predictor

A machine learning web application that predicts the likelihood of diabetes based on diagnostic measurements. The project uses a Logistic Regression model trained on the Pima Indians Diabetes Dataset and is served via a Flask web framework.

## Features

- **Data Preprocessing**: Automated cleaning (dropping non-essential features like 'Pregnancies').
- **Machine Learning**: Logistic Regression model for binary classification.
- **Persistent Model**: Model serialization using pickle for fast loading in production.
- **Web Interface**: User-friendly frontend built with Flask to input health metrics.

## Tech Stack

- **Language**: Python
- **Libraries**: pandas, scikit-learn
- **Deployment**: Flask
- **Model Storage**: Pickle (.pkl)

## Dataset Details

The model is trained on `diabetes.csv`. To optimize performance and focus on physiological metrics, the following features are used:

- Glucose
- Blood Pressure
- Skin Thickness
- Insulin
- BMI
- Diabetes Pedigree Function
- Age

*Note: The 'Pregnancies' column is dropped during the training phase to focus on clinical health indicators.*

## Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/chirag1SF/Diabetes-Predictor.git
cd Diabetes-Predictor
```

### 2. Install Dependencies
```bash
pip install pandas scikit-learn flask
```

### 3. Run the Flask App
```bash
flask run 
```

Open [http://127.0.0.1:5000](http://127.0.0.1:5000) in your browser.
