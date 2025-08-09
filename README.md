# 🌱 Smart Irrigation System using Machine Learning

## 📌 Overview
This project was developed as part of the **Edunet Foundation – AICTE Internship** under the theme **"Automate Irrigation using Soil Moisture and Weather Data"**.  
It leverages **AI/ML** to make intelligent irrigation decisions based on real-time sensor readings, aiming to **optimize water usage** and **improve crop productivity**.

---

## 🎯 Problem Statement
Traditional irrigation systems often lead to **over-watering** or **under-watering** due to the lack of real-time monitoring and decision-making.  
Farmers need an **automated, data-driven solution** that can:
- Analyze environmental and soil conditions
- Predict irrigation needs for multiple land parcels
- Conserve water without compromising crop health

---

## 💡 Solution
Our **Smart Irrigation System**:
- Uses **20 environmental sensors** (soil moisture, humidity, temperature, etc.)
- Predicts irrigation requirements for **3 separate land parcels**
- Employs a **Multi-Output Random Forest Classifier** to generate simultaneous irrigation decisions
- Can be integrated with IoT-based controllers for **real-time automation**

---

## 📂 Dataset
- **File Name:** `irrigation_machine.csv`
- **Records:** 2000 rows
- **Features:** `sensor_0` to `sensor_19` (20 sensor readings)
- **Targets:** `parcel_0`, `parcel_1`, `parcel_2` (binary — 0: No irrigation, 1: Irrigation needed)

---

## 🛠️ Project Workflow

### **Week 1 – Data Exploration & Preprocessing**
- Imported dataset and explored structure (`head()`, `info()`, `describe()`)
- Dropped unnecessary column (`Unnamed: 0`)
- Defined:
  - **X:** Features (`sensor_0` → `sensor_19`)
  - **y:** Labels (`parcel_0` → `parcel_2`)
- Checked data types and distribution

### **Week 2 – Model Development**
- Applied **MinMaxScaler** for normalization
- Used **RandomForestClassifier** wrapped in **MultiOutputClassifier**
- Split data into training/testing sets (`train_test_split`)
- Evaluated predictions using `classification_report`

### **Planned Next Steps**
- Save trained model using **Joblib**
- Deploy via **Streamlit** or **Gradio** for real-time prediction

---

## 📊 Tech Stack
- **Languages:** Python  
- **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn  
- **Tools:** Jupyter Notebook, Joblib  
- **Domain Areas:** AI/ML, Data Analytics, IoT Integration

---

## 🚀 Key Features
- **Multi-Parcel Prediction:** Predicts irrigation needs for multiple areas simultaneously
- **Scalable:** Can be extended for more sensors and parcels
- **IoT-Ready:** Compatible with microcontroller-based water pumps
- **Data-Driven:** Uses machine learning for optimized water usage

---

## 🔧 Improvements Made
- Converted raw CSV into a **clean, structured dataset**
- Implemented **multi-label classification**
- Standardized features for better model performance
- Modularized notebook workflow for easy replication

---

## 📌 Future Scope
- Integrate with **live IoT sensor feeds**
- Build **mobile/web dashboards** for farmers
- Use **weather forecast APIs** to enhance predictions
- Implement **automated pump control** via microcontrollers

---

## 👨‍💻 Author

Aniket Redekar
BE. CSE, 2nd Year
AI/ML Virtual Internship – Edunet Foundation
August 2025
