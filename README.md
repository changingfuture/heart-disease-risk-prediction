# ❤️ Cardio Insight — Heart Disease Risk Prediction

An end-to-end machine learning research project that explores heart disease classification using the UCI Cleveland Heart Disease dataset. Built with Python, Scikit-learn, SHAP and Streamlit.

## 🌐 Live Application

**[Launch Cardio Insight](https://cardio-insight-0.streamlit.app/)**

Cardio Insight is an interactive research demonstration that allows users to enter patient measurements, explore experimental model predictions and understand model behaviour through explainable AI.

> **Disclaimer:** This application is intended exclusively for educational and research purposes. It is not a medical diagnostic tool, and its predictions must not be used for clinical decisions.

---

## 🎯 Project Objectives

- Explore and audit the Cleveland Heart Disease dataset.
- Perform data preprocessing and feature engineering.
- Compare multiple machine learning classification algorithms.
- Perform hyperparameter tuning and model selection.
- Evaluate model performance using nested stratified cross-validation.
- Interpret model behaviour using SHAP and permutation feature importance.
- Develop an interactive web application for research demonstrations.

## 📊 Dataset

**Dataset:** UCI Cleveland Heart Disease Dataset

| Attribute | Details |
|---|---|
| Records | 303 |
| Input features | 13 |
| Problem type | Binary classification |
| Target | Presence or absence of heart disease |

The 13 input features include:

- Age and sex
- Chest pain type
- Resting blood pressure
- Serum cholesterol
- Fasting blood sugar
- Resting ECG
- Maximum heart rate achieved
- Exercise-induced angina
- ST depression (oldpeak)
- Slope of peak exercise ST segment
- Number of major vessels (ca)
- Thalassemia (thal)

## 🧠 Machine Learning Workflow

The project follows a structured machine learning workflow:

1. **Environment and Dataset Audit** — Environment verification, dataset inspection and quality assessment.
2. **Exploratory Data Analysis** — Understanding feature distributions, relationships and patterns.
3. **Data Preprocessing** — Handling numerical and categorical features through preprocessing pipelines.
4. **Model Experiments** — Comparing classification algorithms.
5. **Hyperparameter Tuning** — Searching for suitable model configurations.
6. **Nested Cross-Validation** — Evaluating model selection using five-fold outer cross-validation.
7. **Final Model Selection** — Selecting Logistic Regression as the final candidate.
8. **Model Explainability** — Analysing predictions with SHAP and global feature importance.
9. **Application Development** — Building an interactive Streamlit dashboard.
10. **Deployment** — Publishing the application through Streamlit Community Cloud.

## 📈 Model Evaluation

The selected candidate is **Logistic Regression**.

The saved model metadata reports a best cross-validation ROC-AUC of approximately **0.9210**.

The research workflow includes:

- ROC-AUC
- Accuracy
- Precision
- Recall
- F1-score
- Specificity
- Confusion matrix
- Nested cross-validation results

Cross-validation performance should not be interpreted as a guarantee of performance on unseen populations.

## 🔍 Explainable AI (SHAP)

SHAP (SHapley Additive exPlanations) is integrated to make model behaviour more interpretable.

The application provides:

**Global Explainability**
- Aggregated SHAP feature importance.
- Feature importance visualizations.
- Mean absolute grouped SHAP values.

**Individual Explainability**
- SHAP waterfall explanations.
- Positive and negative feature contributions.
- Individual prediction analysis.

Permutation feature importance is also included as an additional model interpretation technique.

## 🖥️ Application Features

- Interactive patient measurement form.
- Binary heart disease classification.
- Model positive-class output visualization.
- Individual prediction explanations.
- Global feature importance dashboard.
- Research methodology and project information.
- Responsive, multi-page Streamlit interface.

## 🛠️ Technology Stack

| Category | Technologies |
|---|---|
| Programming | Python |
| Data Processing | NumPy, Pandas, SciPy |
| Machine Learning | Scikit-learn |
| Explainable AI | SHAP |
| Visualization | Matplotlib, Seaborn |
| Web Application | Streamlit |
| Model Persistence | Joblib |
| Development | Jupyter Notebook, VS Code |
| Version Control | Git, GitHub |
| Deployment | Streamlit Community Cloud |

## 📁 Project Structure

```text
heart-disease-risk-prediction/
│
├── .streamlit/
│   └── config.toml
│
├── data/
│   ├── raw/
│   └── processed/
│
├── docs/
│
├── models/
│   ├── final_model.joblib
│   └── model_metadata.json
│
├── notebooks/
│   ├── 00_environment_check.ipynb
│   ├── 01_dataset_audit.ipynb
│   ├── 02_model_experiments.ipynb
│   └── 03_model_explainability.ipynb
│
├── reports/
│   ├── baseline_model_comparison.png
│   ├── final_tuning_results.csv
│   ├── nested_cv_summary.csv
│   ├── permutation_feature_importance.png
│   ├── shap_global_importance.png
│   └── shap_summary.png
│
├── src/
│
├── .gitignore
├── app.py
├── requirements.txt
└── README.md
```

*Note: The structure above summarizes the main project components; individual report and source files may vary.*

## ⚙️ Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/changingfuture/heart-disease-risk-prediction.git
cd heart-disease-risk-prediction
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

### 3. Activate the environment

**Windows:**

```bash
.venv\Scripts\activate
```

**Linux/macOS:**

```bash
source .venv/bin/activate
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

Use a compatible Python 3.12 environment and the pinned dependency versions.

### 5. Run the application

```bash
streamlit run app.py
```

Open the local URL displayed in your terminal, usually:

```text
http://localhost:8501
```

## ☁️ Deployment

The application is deployed using Streamlit Community Cloud.

Deployment configuration:

- Repository: `changingfuture/heart-disease-risk-prediction`
- Branch: `main`
- Main application file: `app.py`

To deploy your own fork, connect your GitHub account to Streamlit Community Cloud and select the repository and application entry point.

## ⚠️ Research Limitations

- The project uses a relatively small dataset of 303 records.
- The dataset does not represent every population or clinical setting.
- Model outputs are experimental and are not necessarily clinically calibrated probabilities.
- Feature importance describes model behaviour, not causation.
- The model has not been established as a clinically validated diagnostic system.

This project should be treated as an academic machine learning demonstration, not a substitute for professional medical assessment.

## 🚀 Future Improvements

- External validation using independent datasets.
- More extensive model calibration analysis.
- Additional explainability techniques.
- Improved automated testing.
- Model monitoring and version management.
- Further UI and accessibility improvements.

## 👥 Team and Acknowledgements

This project was developed as a collaborative academic research project.

We acknowledge the contributors involved in dataset analysis, machine learning experimentation, model evaluation, application development and project documentation.

**Dataset acknowledgement:** UCI Machine Learning Repository — Cleveland Heart Disease Dataset.

---

*Built with Python, Scikit-learn, SHAP and Streamlit.*

**Cardio Insight | Heart Disease Risk Prediction Research Project**
