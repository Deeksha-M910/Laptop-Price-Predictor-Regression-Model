# 💻 Laptop Price Predictor

This project predicts the price of a laptop based on user-selected hardware specifications. Built using machine learning techniques, the application allows users to interact with a Streamlit web interface to estimate laptop prices in real-time.

---

## 🔍 Overview

The model is trained on a dataset of laptop specifications and prices. It uses preprocessing pipelines and regression models to make predictions. The frontend is developed using Streamlit for a seamless user experience.

---

## 🚀 Live Demo

👉 [Click here to try the app](https://laptop-price-predictor-regression-model-deeksha.streamlit.app/)  

---

## 📊 Features

Users can choose:
- Brand
- Type of Laptop
- RAM Size
- Laptop Weight
- Touchscreen (Yes/No)
- IPS Display (Yes/No)
- Screen Size
- Screen Resolution
- CPU Brand
- Storage (HDD / SSD)
- GPU Brand
- Operating System

The app then predicts the price based on the selected configuration.

---

## 📁 Dataset

- **Source:** Public dataset of laptop specifications and prices (exact source unknown).
- **Format:** CSV
- **Total Records:** Approximately 1,300 laptops

---

## 🧠 Model & Evaluation

- **Final Model:** XGBoost Regressor (after testing multiple regression algorithms)
- **Preprocessing:** Pipeline with `ColumnTransformer` for encoding and numeric handling
- **Evaluation Metrics:**
  - **R² Score:** ~0.90
  - **MAE:** ~0.14

---

## 🛠 Tech Stack

- Python
- Streamlit — for deploying the model with an interactive UI
- Scikit-learn — for preprocessing, model evaluation, and trying multiple regression algorithms
- XGBoost — selected as the best-performing regression model after comparison
- Pandas, NumPy — for data manipulation and preparation
- Matplotlib, Seaborn — for exploratory data analysis (EDA) and visualization

---

## 🗂 Project Structure

- **app.py**: Streamlit web application
- **df.pkl**: Preprocessed DataFrame used in the app
- **pipe.pkl**: Trained machine learning pipeline (preprocessing + model)
- **laptop_data.csv**: Dataset of laptop specifications and prices
- **requirements.txt**: Python dependencies
- **setup.sh**: Deployment setup script
- **laptop-price-predictor.ipynb**: Jupyter Notebook for EDA and model training

---