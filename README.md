# 🧠 PremiumPredictor AI

An AI-powered web application built with **FastAPI** and **Streamlit** to predict insurance premium categories based on a user's demographics, income, BMI, lifestyle, and occupation.

---

## 🚀 Features

- Predicts insurance premium category: `Low`, `Medium`, or `High`
- Considers factors like age, BMI, smoker status, income, and city tier
- Simple UI built with Streamlit
- Fast backend powered by FastAPI and a pre-trained machine learning model
- Real-time prediction with JSON API and clean responses

---

## 📊 Model Inputs

The app takes the following inputs:

- **Age**  
- **Weight (kg)**  
- **Height (m)**  
- **Annual Income (LPA)**  
- **Smoker status (True/False)**  
- **City name** (used to compute city tier)  
- **Occupation**

---

## 🏗️ Project Structure
```bash
premium_predictor/
├── model.pkl # Pre-trained ML model (classification)
├── main.py # FastAPI backend
├── app.py # Streamlit frontend
├── README.md # You're reading it!
```

---

## 🔧 Setup Instructions

### 1. Clone the repo

```bash
git clone https://github.com/krish9495/PremiumPulse.git
cd PremiumPulse
```
### 2. Run FastAPI server
```bash
uvicorn main:app --reload
```
The API will be available at: http://127.0.0.1:8000

Test it using the interactive docs: http://127.0.0.1:8000/docs

### 4. Run Streamlit frontend
```bash
streamlit run app.py
```
Open http://localhost:8501 in your browser to use the app.


