# 💻 Laptop Price Predictor

This project predicts the price of a laptop based on user-selected hardware specifications. Built using machine learning techniques, the application allows users to interact with a Streamlit web interface to estimate laptop prices in real-time.

## 🔍 Overview

The model is trained on a dataset of laptop specifications and prices. It uses preprocessing pipelines and regression models to make predictions. The frontend is developed using Streamlit for a seamless user experience.

## 🚀 Live Demo

👉 [Click here to try the app](https://your-deployment-link.com)  
_(Replace with actual link if deployed)_

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

## 📁 Dataset

- Source: Self-curated dataset of laptop specifications and prices.
- Format: CSV
- Total Rows: ~1,300

## 🧠 Model

- Model: Gradient Boosting Regressor (via `XGBoost`)
- Pipeline: Includes `ColumnTransformer` with OneHotEncoding and numeric passthrough
- Evaluation:  
  - **R² Score**: ~0.90  
  - **MAE**: ~0.14

## 🛠 Tech Stack

- Python
- Streamlit — for deploying the model with an interactive UI
- Scikit-learn — for preprocessing, model evaluation, and trying multiple regression algorithms
- XGBoost — selected as the best-performing regression model after comparison
- Pandas, NumPy — for data manipulation and preparation
- Matplotlib, Seaborn — for exploratory data analysis (EDA) and visualization

## 🗂 Project Structure

├── app.py # Streamlit web app
├── df.pkl # Cleaned DataFrame used in app
├── pipe.pkl # Trained ML pipeline (preprocessing + model)
├── laptop_data.csv # Original data
├── requirements.txt # Python dependencies
├── setup.sh # Deployment setup script
├── laptop-price-predictor.ipynb # Jupyter notebook (EDA + training)


## ⚙️ Setup Instructions

1. Clone the repository  
   `git clone https://github.com/yourusername/laptop-price-predictor.git`

2. Install dependencies  
   `pip install -r requirements.txt`

3. Run the app  
   `streamlit run app.py`



## 🧑‍💻 Author

**[Deeksha More]**  
_Data Scientist | Machine Learning Enthusiast_

---

