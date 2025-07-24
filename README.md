
# 🌿 Smart Irrigation using Sensor Data

## 📁 Week 1 & Week 2 Progress Report (AI/ML Internship - Edunet Foundation)

---

### 🔍 Problem Statement

Modern irrigation systems require intelligent decision-making based on real-time sensor data to optimize water usage across different parcels of land. This project aims to automate irrigation prediction using machine learning models trained on sensor data.

---

### 📊 Dataset Overview

- **File Used**: `irrigation_machine.csv`
- **Records**: 2000 entries
- **Features**:
  - `sensor_0` to `sensor_19`: Sensor readings from various environmental and soil condition devices.
- **Labels**:
  - `parcel_0`, `parcel_1`, `parcel_2`: Indicates irrigation status for each of the 3 parcels (binary: 0 or 1).

---

### ✅ Tasks Completed

#### 📅 Week 1

- Imported essential libraries: `pandas`, `matplotlib`, `seaborn`, `scikit-learn`, `joblib`.
- Loaded and explored the dataset.
- Dropped unnecessary column `Unnamed: 0`.
- Printed data types and verified there are no missing values.
- Generated statistical summaries using `.describe()`.
- Split data into:
  - `X` (features): sensor data (`sensor_0` to `sensor_19`)
  - `y` (labels): target parcels (`parcel_0`, `parcel_1`, `parcel_2`)
- Verified dimensions of `X` and `y`.

#### 📅 Week 2

- Prepared initial structure for model training.
- Imported `RandomForestClassifier` and `MultiOutputClassifier`.
- Prepared to use `train_test_split` and `MinMaxScaler` (model training not executed yet).

---

### 🔧 Next Steps (Planned for Week 3)

- Apply feature scaling using `MinMaxScaler`.
- Train a multi-output classifier using `RandomForestClassifier`.
- Evaluate model performance using `classification_report`.
- Save the trained model using `joblib`.

---

### 📌 Notes

- No preprocessing (like normalization or feature engineering) has been applied yet.
- Model training and evaluation are pending.
- Improvement suggestions from Week 1 are noted but not yet implemented.

---

### 🧠 Tools & Libraries

- Python
- Pandas, Matplotlib, Seaborn
- Scikit-learn (Random Forest, Multi-output classifier)
- Google Colab
