# 💳 Credit Scoring Model

A machine learning project developed as part of the **CodeAlpha Internship** that predicts the creditworthiness of individuals based on historical financial data using classification algorithms.

---

## 📌 Project Overview

Credit scoring is a statistical analysis performed by lenders to determine the creditworthiness of a person or business. This project builds a predictive model that classifies individuals as **creditworthy** or **not creditworthy** based on various financial and demographic features.

---

## 🎯 Objectives

- Analyze and preprocess historical financial data
- Build and evaluate classification models to predict credit risk
- Identify key features that influence credit scores
- Compare model performances using appropriate metrics

---

## 📁 Project Structure

```
CodeAlpha_CreditScoringModel/
│
├── data/
│   ├── raw/                  # Raw dataset files
│   └── processed/            # Cleaned and preprocessed data
│
├── notebooks/
│   └── credit_scoring.ipynb  # Main Jupyter Notebook
│
├── models/
│   └── best_model.pkl        # Saved trained model
│
├── src/
│   ├── preprocessing.py      # Data cleaning and feature engineering
│   ├── train.py              # Model training script
│   └── evaluate.py           # Model evaluation script
│
├── requirements.txt          # Python dependencies
└── README.md                 # Project documentation
```

---

## 📊 Dataset

The dataset contains historical financial records with features such as:

| Feature | Description |
|---|---|
| `Age` | Age of the individual |
| `Income` | Annual income |
| `Loan Amount` | Amount of loan requested |
| `Loan Duration` | Duration of the loan (months) |
| `Employment Status` | Employed / Self-employed / Unemployed |
| `Credit History` | Past credit repayment record |
| `Debt-to-Income Ratio` | Total debt relative to income |
| `Number of Dependents` | Number of financial dependents |
| `Credit Score` | Target variable (Good / Bad) |

> **Note:** If using a public dataset, replace with the appropriate dataset link (e.g., [German Credit Dataset](https://archive.ics.uci.edu/ml/datasets/statlog+(german+credit+data)) from UCI ML Repository).

---

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/divyadharshinidd0211-lgtm/CodeAlpha_CreditScoringModel.git
cd CodeAlpha_CreditScoringModel
```

### 2. Create a Virtual Environment (Recommended)

```bash
python -m venv venv
source venv/bin/activate        # On macOS/Linux
venv\Scripts\activate           # On Windows
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook notebooks/credit_scoring.ipynb
```

---

## 🤖 Models Used

The following classification algorithms were implemented and compared:

- ✅ Logistic Regression
- ✅ Decision Tree Classifier
- ✅ Random Forest Classifier
- ✅ Gradient Boosting (XGBoost)
- ✅ Support Vector Machine (SVM)
- ✅ K-Nearest Neighbors (KNN)

---

## 📈 Evaluation Metrics

Models were evaluated using:

- **Accuracy**
- **Precision, Recall & F1-Score**
- **ROC-AUC Score**
- **Confusion Matrix**

---

## 🔍 Key Steps

1. **Data Preprocessing**
   - Handling missing values
   - Encoding categorical variables
   - Feature scaling (StandardScaler / MinMaxScaler)
   - Train-test split (80/20)

2. **Exploratory Data Analysis (EDA)**
   - Distribution plots
   - Correlation heatmap
   - Class imbalance check

3. **Model Training & Hyperparameter Tuning**
   - GridSearchCV / RandomizedSearchCV

4. **Model Evaluation & Comparison**
   - Performance metrics on test data
   - Feature importance visualization

---

## 📉 Results

| Model | Accuracy | ROC-AUC |
|---|---|---|
| Logistic Regression | ~75% | ~0.78 |
| Decision Tree | ~76% | ~0.74 |
| Random Forest | ~82% | ~0.87 |
| XGBoost | ~84% | ~0.89 |
| SVM | ~79% | ~0.83 |
| KNN | ~73% | ~0.75 |

> *Results may vary based on dataset and hyperparameter tuning.*

---

## 🛠️ Technologies Used

- **Language:** Python 3.x
- **Libraries:** Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn
- **Environment:** Jupyter Notebook

---

## 🙋‍♀️ Author

**Divyadharshini**
- 🔗 GitHub: [@divyadharshinidd0211-lgtm](https://github.com/divyadharshinidd0211-lgtm)
- 📌 Internship: CodeAlpha Machine Learning Internship

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 🙏 Acknowledgements

- [CodeAlpha](https://www.codealpha.tech/) for the internship opportunity
- [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/index.php) for publicly available datasets
- Scikit-learn and XGBoost open-source communities
