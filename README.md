# Flight-Delay-Prediction-using-Big-Data
✈️ Flight Delay Prediction
This project analyzes and predicts flight delays using real-world U.S. flight data. The goal is to build a classification model that can determine whether a flight will be delayed by more than 15 minutes.

📁 Datasets Used
flights.csv: Flight-level data (departure, arrival times, delays, etc.)

airports.csv: Information about airport locations

airlines.csv: Information about airlines

🛠️ Project Workflow
1. Data Loading & Inspection
Load and inspect the data for basic structure, size, and missing values.

2. Data Cleaning & Feature Engineering
Drop rows with critical missing values.

Convert times to readable format.

Create custom features like DELAY_CATEGORY, DAY_PERIOD.

3. Exploratory Data Analysis (EDA)
Visualize:

Number of flights per airline

Delay distributions

Delay by time of day

Delay categories by airline

4. Predictive Modeling
Model: Random Forest Classifier

Target: Whether a flight is delayed (ARRIVAL_DELAY > 15 mins)

Evaluation: Accuracy, Confusion Matrix, Classification Report

5. Model Improvement
Apply SMOTE to balance the dataset

Evaluate model using ROC AUC, Precision-Recall Curve

6. Model Saving
Final model is saved using joblib as flight_delay_rf_model.pkl.

📊 Model Performance
Accuracy: ~75.8%

ROC AUC: 0.83

Balanced F1-scores for both classes using SMOTE.

📦 Libraries Used
pandas, numpy, matplotlib, seaborn

scikit-learn, imbalanced-learn

joblib for model serialization

👩‍💻 Authors
Ons Tohari


📌 Notes
This project was developed and tested in Google Colab.

Datasets are not included in the repo due to size limitations. Make sure to update the file paths accordingly.
