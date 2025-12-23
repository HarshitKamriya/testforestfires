# 🔥 Algerian Forest Fire Prediction using Ridge Regression

## 📌 Project Overview
This project focuses on predicting forest fire occurrences in Algeria using the **Algerian Forest Fire Dataset**.  
The dataset contains meteorological and fire-related attributes collected from two regions (Bejaia and Sidi Bel-abbes) between June–September 2012.  

I experimented with multiple regression techniques:
- Linear Regression
- Lasso Regression
- Elastic Net Regression
- Ridge Regression ✅ (selected due to highest accuracy)

The final Ridge Regression model was serialized into a `.pkl` file and integrated into a **Flask web application** with HTML templates. The app is now ready for deployment on **AWS**.

---

## 📂 Dataset
- **Name:** Algerian Forest Fire Dataset  
- **Attributes:** Temperature, RH (Relative Humidity), Wind, Rain, FFMC, DMC, DC, ISI, BUI, FWI, Classes (fire/no fire)  

---

## ⚙️ Tech Stack
- **Python** (Data preprocessing, model training)
- **Scikit-learn** (Regression models, Ridge Regression)
- **Flask** (Web framework)
- **HTML/CSS** (Frontend templates)
- **Pickle (.pkl)** (Model serialization)
- **AWS EC2 / Elastic Beanstalk** (Deployment)

---

## 🚀 Workflow
1. **Data Preprocessing**
   - Cleaned dataset (handled missing values, normalized features).
   - Split into training and testing sets.

2. **Model Training**
   - Compared Linear, Lasso, Elastic Net, and Ridge Regression.
   - Ridge Regression achieved the best accuracy.

3. **Model Serialization**
   - Saved trained Ridge model as `model.pkl`.

4. **Web Application**
   - Built Flask app with routes for prediction.
   - HTML templates for user input and result display.

5. **Deployment**
   - Prepared app for deployment on AWS (requirements.txt, Procfile, etc.).

---

## 📊 Results
- **Ridge Regression Accuracy:** ~ Highest among tested models.
- **Performance Metrics:** R², MAE, RMSE :
                                R2 Score 0.9842993364555513
                                Mean absolute error 0.564230534010569
                                RMSE Score 0.6949198918152072

---

