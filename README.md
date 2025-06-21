# Flight-Delay-Prediction-using-Big-Data
<h1 align="center">✈️ Flight Delay Prediction</h1>
<p align="center">
  <b>Analyze, Visualize, and Predict Flight Delays with Machine Learning</b><br>
  <i>Built using Python, scikit-learn, pandas, and visualized with seaborn/matplotlib</i>
</p>

---

## 📁 Datasets Used

| Dataset       | Description                               |
|---------------|-------------------------------------------|
| `flights.csv` | Flight details (delays, times, airports)  |
| `airports.csv`| Info about U.S. airports                  |
| `airlines.csv`| Airline codes and names                   |

---

## 🔄 Project Workflow

### 1️⃣ Data Loading & Inspection
- Load CSVs from Google Drive
- Print shapes, columns, and missing values

### 2️⃣ Data Cleaning & Feature Engineering
- Drop incomplete rows
- Create time features (convert HHMM → HH:MM)
- Add: `DELAY_CATEGORY`, `DAY_PERIOD`

### 3️⃣ Exploratory Data Analysis (EDA)
Visualizations:
- 🧮 Flights per Airline
- 🏙️ Top 10 Busiest Airports
- ⏱️ Delay Distributions
- 🕒 Delay by Time of Day
- 🏷️ Delay Categories by Airline

### 4️⃣ Predictive Modeling
- Binary classification:
  - `1 = delayed > 15 mins`
  - `0 = on-time / early`
- Model: **Random Forest**
- SMOTE for balancing classes

### 5️⃣ Evaluation Metrics

| Metric       | Value      |
|--------------|------------|
| Accuracy     | 75.8%      |
| ROC AUC      | 0.83       |
| F1-score     | Balanced   |

Visuals:
- ROC Curve
- Precision-Recall Curve
- Confusion Matrix

### 6️⃣ Final Model
- Saved as: `flight_delay_rf_model.pkl` using `joblib`

---

## 🧰 Tech Stack

```bash
Python, pandas, numpy
scikit-learn, imbalanced-learn
matplotlib, seaborn
Google Colab
