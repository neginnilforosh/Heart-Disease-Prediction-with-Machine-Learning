# 🫀 Heart Disease Prediction Machine Learning Project

An end-to-end Machine Learning pipeline designed to classify and predict the presence of heart disease using clinical patient attributes. This project covers data ingestion, exploratory data analysis (EDA), feature scaling, baseline model training, evaluation, and hyperparameter tuning.

---

## 📌 Table of Contents
- [Project Overview](#-project-overview)
- [Dataset Description](#-dataset-description)
- [Project Architecture & Workflow](#-project-architecture--workflow)
- [Technologies Used](#-technologies-used)
- [Installation & Setup](#-installation--setup)
- [Usage](#-usage)
- [Model Evaluation & Results](#-model-evaluation--results)
- [Future Improvements](#-future-improvements)
- [License](#-license)

---

## 🩺 Project Overview
Cardiovascular diseases are a primary cause of global health issues. Early detection through predictive modeling can assist medical professionals in identifying high-risk patients. 

This project leverages clinical datasets to train machine learning classifiers—including Logistic Regression, Random Forest, Support Vector Machines (SVM), and K-Nearest Neighbors (KNN)—to accurately predict whether a patient has heart disease based on medical indicators.

---

## 📊 Dataset Description
The dataset is retrieved from Kaggle (`johnsmith88/heart-disease-dataset`) and contains key clinical parameters:

| Feature | Type | Description |
| :--- | :--- | :--- |
| `age` | Numeric | Patient age in years |
| `sex` | Categorical | Sex (1 = male; 0 = female) |
| `cp` | Categorical | Chest pain type (0: Typical Angina, 1: Atypical Angina, 2: Non-anginal, 3: Asymptomatic) |
| `trestbps` | Numeric | Resting blood pressure (in mm Hg on admission) |
| `chol` | Numeric | Serum cholesterol level in mg/dl |
| `fbs` | Categorical | Fasting blood sugar > 120 mg/dl (1 = true; 0 = false) |
| `restecg` | Categorical | Resting electrocardiographic results (0, 1, 2) |
| `thalach` | Numeric | Maximum heart rate achieved |
| `exang` | Categorical | Exercise-induced angina (1 = yes; 0 = no) |
| `oldpeak` | Numeric | ST depression induced by exercise relative to rest |
| `slope` | Categorical | Slope of the peak exercise ST segment |
| `ca` | Numeric | Number of major vessels (0–3) colored by fluoroscopy |
| `thal` | Categorical | Thalassemia type (1 = normal; 2 = fixed defect; 3 = reversible defect) |
| **`target`** | **Binary Target** | **Heart disease status (1 = presence, 0 = absence)** |

---

## ⚙️ Project Architecture & Workflow

1. **Data Ingestion**: Programmatically retrieving data via `kagglehub`.
2. **Exploratory Data Analysis (EDA)**: Analyzing feature distributions, correlation heatmaps, missing values, and outliers using `seaborn` and `matplotlib`.
3. **Data Preprocessing**: Scaling numerical variables via `StandardScaler` and handling categorical encodings.
4. **Model Training**: Implementing baseline models (Logistic Regression, Decision Tree, Random Forest, SVM, KNN).
5. **Model Evaluation**: Metrics breakdown using Accuracy, Precision, Recall, F1-Score, and ROC-AUC curves.
6. **Hyperparameter Tuning**: Optimizing top-performing classifiers using `GridSearchCV`.

---

## 🛠️ Technologies Used
- **Language:** Python 3.9+
- **Data Wrangling:** `pandas`, `numpy`
- **Visualization:** `matplotlib`, `seaborn`
- **Machine Learning:** `scikit-learn`
- **Dataset Retrieval:** `kagglehub`

---

## 💻 Installation & Setup

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/YOUR-USERNAME/heart-disease-prediction.git
   cd heart-disease-prediction
   ```

2. **Create a Virtual Environment (Optional):**
   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

---

## 🚀 Usage

Run the Jupyter Notebook to step through data preprocessing, visualization, and model execution:

```bash
jupyter notebook ML_Basic.ipynb
```

---

## 📈 Model Evaluation & Results

Summary of performance metrics across tested classification algorithms:

| Model | Accuracy | Precision | Recall | F1-Score |
| :--- | :--- | :--- | :--- | :--- |
| **Logistic Regression** | 85% | 0.83 | 0.88 | 0.85 |
| **Random Forest** | 90% | 0.88 | 0.92 | 0.90 |
| **Support Vector Machine (SVM)** | 86% | 0.84 | 0.87 | 0.85 |
| **K-Nearest Neighbors (KNN)** | 83% | 0.81 | 0.84 | 0.82 |

*(Note: Replace sample metrics above with your notebook's exact test scores).*

---

## 🔮 Future Improvements
- Build an interactive web frontend using **Streamlit** or **Flask** for real-time predictions.
- Integrate model explainability frameworks (**SHAP** or **LIME**).
- Benchmark advanced gradient boosting algorithms like **XGBoost** and **LightGBM**.

---

## 📄 License
This project is open-source and available under the [MIT License](LICENSE).
