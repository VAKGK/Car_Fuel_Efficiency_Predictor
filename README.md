# 🚗 Car Mileage Prediction

### **Estimating Fuel Efficiency with Machine Learning**

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Scikit-Learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)](https://streamlit.io/)
[![Live App](https://img.shields.io/badge/Live-App-success?style=for-the-badge&logo=streamlit)](https://carmpgpredictions.streamlit.app/)

---

## 📖 Overview

**Fuel efficiency is a critical factor in automotive design and consumer choice.**

This project utilizes a **Machine Learning Regression** model to predict the Miles Per Gallon (MPG) of a vehicle based on its technical specifications. By analyzing features such as cylinders, displacement, horsepower, and weight, the model provides an accurate estimation of fuel consumption.

The final model is deployed as an interactive **Streamlit Web Application**, allowing users to input car specs and get real-time mileage predictions.

> *"Driving insights into vehicle efficiency."*

---

## 📱 Web App Features

Experience the model in action through the live dashboard:

👉 **[Launch the App](https://carmpgpredictions.streamlit.app/)**

* **⚡ Real-Time Prediction:** Instant MPG calculation based on user inputs.
* **🎛️ Preset Profiles:** Quickly test the model with standard vehicle configurations.
* **🎨 Professional UI:** A polished interface with hover effects and a responsive design.
* **❓ Help Section:** Detailed feature explanations in expandable tabs for better user guidance.

---

## 📊 Model Performance

The Linear Regression model was evaluated on a test dataset to ensure accuracy:

* **R² Score:** `0.85` (Strong correlation between features and target)
* **MAE (Mean Absolute Error):** `2.25`
* **MSE (Mean Squared Error):** `8.20`

---

## 🛠️ Tools & Technologies Used

* **🐍 Python:** Core language for analysis and modeling.
* **🐼 Pandas & NumPy:** Used for data manipulation and numerical calculations.
* **📉 Seaborn & Matplotlib:** Used for exploratory data analysis (EDA) and visualizing correlations.
* **🤖 Scikit-Learn:** Used for data scaling, model training, and evaluation.
* **📦 Joblib:** Used for serializing (saving) the trained model and scaler.
* **🌐 Streamlit:** Used to build and deploy the frontend application.

---

## ⚙️ The Workflow (Pipeline)

The project follows a standard Machine Learning pipeline from raw data to a deployed app.

```mermaid
graph TD;
    A["📂 Raw Auto Data\n(CSV)"] -->|Cleaning & Handling Missing Values| B{"⚙️ Preprocessing\n(Pandas)"};
    B -->|Feature Scaling| C["⚖️ Standardization\n(StandardScaler)"];
    C -->|Training| D["🧠 Linear Regression\n(Scikit-Learn)"];
    D -->|Evaluation| E["📊 Model Metrics\n(R²: 0.85, MAE: 2.25)"];
    E -->|Deployment| F["🌐 Streamlit Web App\n(Real-time Prediction)"];

    style A fill:#f9f,stroke:#333,stroke-width:2px
    style D fill:#bbf,stroke:#333,stroke-width:2px
    style F fill:#bfb,stroke:#333,stroke-width:2px
