# 🏥 Health Insurance Cost Predictor – ML-Based Medical Premium Estimator

<p align="center">
  Predict individual health insurance charges using demographics and lifestyle data — deployed as a real-time web app for instant cost estimation.
</p>

---

## 📌 Project Overview

This project is designed to predict **health insurance charges** based on user input such as age, gender, BMI, smoking habits, and more.  
It enables **insurance providers** and **consumers** to estimate potential premiums using **machine learning models** trained on real-world data.

> ✅ Built using the **Medical Cost Personal Dataset**, achieving:  
> - 🔍 **R² Score > 0.988**  
> - ⚙️ Deployed with **Streamlit** for a user-friendly experience

---

## 📊 Key Highlights

- 🧮 Predicts medical insurance charges using:
  - Age, Sex, BMI
  - Number of children
  - Smoking status
  - Region of residence
- ⚙️ Model trained using **Linear Regression**, **Random Forest**, and **XGBoost**
- 🛠️ Hyperparameter tuning for improved accuracy
- 💡 Deployed via **Streamlit web app** for instant predictions

### ✅ Results

- 🧠 Developed a machine learning model using **50,000+ records**, achieving an **R² score of 0.988** for health insurance premium prediction.
- 📉 Reduced extreme prediction errors for users under age 25 from **73% to 2%** using **age-based segmentation** and retraining with additional features.
- 🔧 Executed **10+ preprocessing steps** including:
  - Outlier removal
  - Feature engineering
  - Encoding techniques
  - **VIF-based feature reduction** to eliminate multicollinearity
- ⚡ Deployed final model as a **real-time Streamlit app**, enabling predictions in **under 1 second** with **age-specific model selection** logic.

---

---

## 🖼️ App UI Preview

<p align="center">
  <img src="images/ui_screenshot.png" alt="Health Insurance Predictor UI" width="700"/>
</p>

```

---

## 🧠 How It Works

1. **User Inputs:** Age, Gender, BMI, Children, Smoking Status, Region  
2. **Model Prediction:** Pre-trained ML model estimates insurance charges  
3. **Output Display:** Estimated premium amount is displayed instantly

---

## 🛠️ Tools & Technologies

| Category          | Tools                                    |
|------------------|------------------------------------------|
| 🐍 Programming    | Python                                   |
| 📊 Data Handling  | Pandas, NumPy                            |
| 🤖 Machine Learning | Scikit-learn, XGBoost, Random Forest       |
| 📉 Visualization  | Matplotlib, Seaborn                      |
| 📦 Model Saving   | Joblib                                   |
| 🌐 Deployment     | Streamlit                                |
| 📓 Development    | Jupyter Notebooks                        |

---

## 🚀 How to Run Locally  

1. **Clone the repository**  
   ```bash
   git clone https://github.com/Dheeraj23-08/Health_insurance_predictor_1.git
   cd Health_insurance_predictor_1
   ```

2. **Install dependencies**  
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Streamlit app**  
   ```bash
   streamlit run app/main.py
   ```

---

## 📺 Live Demo

🔗 *[click here to ptredit your health insurance plan]*

