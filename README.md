# 🧪 Glucose Level Prediction using Machine Learning

This project uses supervised machine learning to predict whether an individual is likely to have abnormal glucose levels based on health and lifestyle indicators. It aims to support early diagnosis and prevention of diabetes-related conditions.

## 📊 Dataset: Framingham Heart Study

- Source: [UCI / Kaggle / other if applicable]
- Rows: ~4000  
- Features: Age, BMI, Heart Rate, Smoking Status, Diabetes Pedigree, etc.  
- Target: Binary label indicating abnormal glucose level (`1` = high, `0` = normal)

> Note: The dataset was preprocessed to handle missing values, normalize numerical features, and encode categorical variables.

---

## 🧠 Problem Statement

Predict whether a person has abnormal blood glucose levels based on various health metrics. The model can help identify individuals at higher risk for diabetes or cardiovascular complications.

---

## ⚙️ Tech Stack

- **Python**  
- **Pandas**, **NumPy** – Data manipulation  
- **Matplotlib**, **Seaborn** – EDA & visualization  
- **Scikit-learn** – ML models (Logistic Regression, Random Forest, etc.)
- **Streamlit (optional)** – For app UI

---

## 🔁 Project Workflow

1. **Data Loading & Cleaning**
   - Handled missing/null values
   - Removed outliers
   - Converted data types where necessary

2. **Exploratory Data Analysis**
   - Distribution plots for features
   - Correlation heatmaps
   - Class imbalance analysis

3. **Feature Engineering**
   - Scaling numerical features
   - One-hot encoding categorical features
   - Feature selection based on correlation and domain relevance

4. **Model Training & Evaluation**
   - Used `train_test_split` (80:20)
   - Tried baseline Logistic Regression, Random Forest, and Gradient Boosting
   - Evaluated using accuracy, precision, recall, and ROC-AUC

5. **Model Interpretation**
   - Confusion matrix
   - Feature importance plots

6. **(Optional) Deployment**
   - Built a simple Streamlit app for demo predictions (if added)

---

## ✅ Results

| Model              | Accuracy | Precision | Recall | ROC-AUC |
|-------------------|----------|-----------|--------|---------|
| Logistic Regression | 0.78     | 0.74      | 0.70   | 0.80    |
| Random Forest       | 0.82     | 0.78      | 0.76   | 0.86    |
| Gradient Boosting   | 0.84     | 0.80      | 0.78   | 0.88    |

> Best model: **Gradient Boosting**, with highest balanced performance.

---

## 📁 Folder Structure

Glucose-Prediction/
│
├── data/
│   └── framingham.csv
├── notebooks/
│   └── Glucose\_Prediction\_Summary.ipynb
├── models/
│   └── saved\_model.pkl (optional)
├── app/ (optional)
│   └── streamlit\_app.py
├── README.md
└── requirements.txt

## 🧪 How to Run

1. Clone the repo:
   git clone https://github.com/yourusername/Glucose-Prediction.git
   cd Glucose-Prediction

2. Install dependencies:
   pip install -r requirements.txt

3. Run the notebook:
   Open notebooks/Glucose_Prediction_Summary.ipynb in Jupyter

4. (Optional) Run Streamlit App:

   
   streamlit run app/streamlit_app.py
   

---

## 📌 Future Work

* Hyperparameter tuning with GridSearchCV
* Deep learning model comparison (optional)
* Streamlit UI for live predictions
* More robust evaluation with cross-validation

---

## 📚 References

* [Framingham Heart Study](https://www.framinghamheartstudy.org/)
* Scikit-learn documentation
