
# 🧠 Parkinson's Disease Detection using Machine Learning

This repository presents a machine learning project that aims to **detect Parkinson's Disease using voice measurement data**. Parkinson’s is a **progressive neurological disorder** that affects movement and speech. Detecting it early can greatly enhance a patient’s quality of life through timely treatment.

---

## 📊 Problem Statement

The primary objective of this project is to **classify individuals as either healthy or affected by Parkinson’s Disease** based on various biomedical voice measurements. By analyzing vocal attributes, machine learning models can identify patterns associated with the disease.

---

## 📁 Dataset Overview

- **Source**: [Kaggle – Parkinson Disease Detection Dataset](https://www.kaggle.com/datasets/jainaru/parkinson-disease-detection)  
- **Total Instances**: 195  
- **Total Features**: 22 biomedical voice features + 1 target column  
- **Target Column**: `status`  
  - `1` → Parkinson’s Disease  
  - `0` → Healthy  

Each row in the dataset represents **voice measurements from a single individual**, extracted from sustained phonations.

---

## 🔬 Feature Descriptions

Key features used for detection include:

| Feature Name         | Description                                        |
|----------------------|----------------------------------------------------|
| `MDVP:Fo(Hz)`        | Average vocal fundamental frequency                |
| `MDVP:Jitter(%)`     | Frequency variation in voice                       |
| `MDVP:Shimmer`       | Amplitude variation in voice                       |
| `NHR`, `HNR`         | Noise-to-Harmonics and Harmonics-to-Noise Ratios  |
| `spread1`, `spread2` | Nonlinear measures of variation in the signal      |
| `DFA`, `PPE`         | Additional nonlinear features capturing complexity |

---

## ⚙️ Technologies Used

The following tools and libraries were used throughout the project:

- **Python**
- **Scikit-learn**
- **XGBoost**
- **Pandas**, **NumPy**
- **Matplotlib**, **Seaborn**

---

## 🚀 Workflow Steps

The complete machine learning pipeline includes:

1. **Data Cleaning & Preprocessing**
2. **Exploratory Data Analysis (EDA)**
3. **Feature Scaling** using `StandardScaler`
4. **Train-Test Split** (80% training, 20% testing)
5. **Model Training** using the **XGBoost Classifier**
6. **Model Evaluation** using classification metrics & visualizations

---

## 📈 Evaluation Metrics

Model performance was assessed using:

- **Accuracy**
- **Precision**
- **Recall**
- **F1 Score**
- **Confusion Matrix**
- **ROC-AUC Curve**

---

## ✅ XGBoost Model Results

| Metric            | Score  |
|-------------------|--------|
| Accuracy          | 0.94   |
| Precision         | 0.94   |
| Recall            | 1.00   |
| F1 Score          | 0.97   |
| ROC-AUC Score     | ~0.98  |

---

## 📊 Confusion Matrix

|                        | Predicted: Healthy | Predicted: Parkinson’s |
|------------------------|--------------------|-------------------------|
| **Actual: Healthy**    | 5                  | 2                       |
| **Actual: Parkinson’s**| 0                  | 32                      |

The model **successfully identified all patients with Parkinson’s** and only produced **2 false positives**.

---

## 📌 Role of Machine Learning in Parkinson’s Detection

Parkinson’s disease often causes **subtle changes in speech patterns**, which are hard to detect early through traditional clinical methods. Machine learning can:

- Analyze complex vocal biomarkers
- Detect early signs **before physical symptoms are apparent**
- Provide a **fast, cost-effective pre-screening tool** for clinicians

---

## 📉 Visualizations Included

To support insights and model interpretation, the project features:

- 📌 **Correlation Heatmap** of features  
- 📌 **Feature Importance Plot** (Horizontal bar chart)  
- 📌 **Model Comparison Plot**  
- 📌 **Confusion Matrix Visuals** for each classifier

---

## 🔍 Conclusion

The **XGBoost classifier** achieved:

- **94% Accuracy**
- **100% Recall**

This makes it a highly reliable model for identifying Parkinson’s Disease using voice data. The approach has strong potential as a **non-invasive diagnostic aid** in clinical settings.

---

## 📁 Project Structure

```plaintext
📦 Parkinsons-Disease-Detection/
├── parkinsons.ipynb     # Full model implementation in Jupyter Notebook
├── README.md            # Project overview and documentation
```

---

## 👨‍💻 Developed by

**Muhammad Adnan Khan**

Feel free to connect for feedback, suggestions, or collaborations!
