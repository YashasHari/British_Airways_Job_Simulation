
# ✈️ British Airways Data Science Simulation (Forage)

This project is a simulation of a data science task for British Airways, created as part of the [Forage virtual experience](https://www.theforage.com/). The task focuses on predicting whether a customer completes a booking based on their booking data using classification techniques.

---

## 🎯 Objective

- Analyze and preprocess customer booking data.
- Build a predictive model to classify booking completion.
- Evaluate model performance using various metrics.
- Identify key features influencing booking completion.

---

## 🔑 Key Steps

1. *Data Loading and Exploration*
   - Load dataset and inspect its shape, data types, and missing values.
   - Understand sample data to inform preprocessing.

2. *Data Preprocessing*
   - Encode categorical variables with Label Encoding.
   - Engineer cyclical features for flight_hour using sine and cosine transformations.
   - Drop the original flight_hour column.

3. *Modeling*
   - Split data into training and testing sets.
   - Train a Random Forest Classifier on the training data.
   
4. *Evaluation*
   - Predict on the test set.
   - Assess model performance using accuracy, ROC AUC, confusion matrix, and classification report.
   - Perform 5-fold cross-validation to verify model stability.

5. *Feature Importance*
   - Visualize feature importance from the Random Forest model to understand influential predictors.

---

## 🛠️ Tools & Libraries Used

- *Data Handling & Analysis:* pandas, numpy
- *Visualization:* matplotlib, seaborn
- *Preprocessing & Modeling:* scikit-learn
  - Label Encoding
  - Train-test splitting
  - Random Forest Classifier
  - Cross-validation
- *Evaluation Metrics:* Accuracy, ROC AUC, Confusion Matrix, Classification Report

---

## 📁 Files

- british_airways_simulation.ipynb — Main notebook for data preprocessing, modeling, and evaluation.
- README.md — This file.
  
---

## 🚀 Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/british-airways-simulation.git
   cd british-airways-simulation
   ```

2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```

3. Download the dataset from the Forage platform and update the path in the notebook:
   ```python
   df = pd.read_csv("path/to/customer_booking.csv", encoding='ISO-8859-1')
   ```

4. Run the notebook:
   ```bash
   jupyter notebook british_airways_simulation.ipynb
   ```

---

## 📊 Output Sample

- Evaluation metrics (Accuracy, ROC AUC)
- Feature importance visualization
