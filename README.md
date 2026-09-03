# Customer Churn Prediction

A comprehensive data analysis project that predicts customer churn using SQL and Python. This project demonstrates end-to-end data science workflow including data extraction, exploratory data analysis, feature engineering, and machine learning model development.

## 📋 Table of Contents

- [Overview](#overview)
- [Project Structure](#project-structure)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Technologies](#technologies)
- [Key Findings](#key-findings)
- [Future Improvements](#future-improvements)

## 🎯 Overview

**Objective:** Build a predictive model to identify customers likely to churn, enabling proactive retention strategies.

**Business Impact:**
- Identify at-risk customers before they leave
- Optimize retention marketing campaigns
- Reduce customer acquisition costs
- Improve customer lifetime value

## 📁 Project Structure

```
customer-churn-analysis/
├── data/
│   ├── raw/                 # Original, immutable data
│   └── processed/           # Cleaned and transformed data
├── notebooks/
│   ├── 01_exploratory_analysis.ipynb
│   ├── 02_data_preprocessing.ipynb
│   ├── 03_feature_engineering.ipynb
│   └── 04_model_development.ipynb
├── sql/
│   ├── data_extraction.sql  # Extract raw data from database
│   ├── data_validation.sql  # Data quality checks
│   └── feature_queries.sql  # Feature computation queries
├── src/
│   ├── data_loader.py       # Data extraction and loading
│   ├── preprocessing.py     # Data cleaning and transformation
│   ├── feature_engineering.py # Feature creation
│   ├── model_training.py    # Model training and evaluation
│   └── utils.py             # Utility functions
├── models/
│   └── churn_model.pkl      # Trained model artifact
├── reports/
│   ├── figures/             # Generated visualizations
│   └── analysis_report.md   # Summary findings
├── tests/
│   ├── test_preprocessing.py
│   └── test_features.py
├── requirements.txt         # Python dependencies
├── .gitignore              # Git ignore patterns
├── config.yaml             # Configuration parameters
└── README.md               # This file
```

## 📊 Dataset

- **Source:** [Specify data source]
- **Records:** [Number of customer records]
- **Features:** [Number of features]
- **Target Variable:** Churn (Binary: Yes/No)
- **Time Period:** [Date range]

### Key Features:
- Customer demographics (age, gender, location)
- Account information (tenure, subscription type)
- Service usage metrics (call frequency, data consumption)
- Billing information (monthly charges, contract type)
- Customer support interactions

## 🔍 Methodology

### 1. **Data Extraction (SQL)**
   - Query customer data from database
   - Join multiple tables for comprehensive features
   - Data validation and quality checks

### 2. **Exploratory Data Analysis (EDA)**
   - Univariate analysis of each feature
   - Bivariate analysis with churn target
   - Correlation analysis
   - Distribution analysis and outlier detection

### 3. **Data Preprocessing**
   - Handling missing values
   - Outlier treatment
   - Encoding categorical variables
   - Feature scaling and normalization

### 4. **Feature Engineering**
   - Creating interaction features
   - Aggregating temporal data
   - Deriving domain-specific features
   - Feature selection using statistical methods

### 5. **Model Development**
   - Multiple algorithms tested:
     - Logistic Regression
     - Random Forest
     - Gradient Boosting
     - Neural Networks
   - Hyperparameter tuning
   - Cross-validation and model evaluation

### 6. **Model Evaluation**
   - Metrics: Accuracy, Precision, Recall, F1-Score, AUC-ROC
   - Confusion matrix analysis
   - Feature importance analysis
   - Business impact assessment

## 💻 Installation

### Prerequisites
- Python 3.8+
- SQL database access
- Git

### Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/bappaditya27/customer-churn-analysis.git
   cd customer-churn-analysis
   ```

2. **Create virtual environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Configure database connection:**
   - Update `config.yaml` with your database credentials
   - Ensure proper permissions for SQL queries

## 🚀 Usage

### 1. Extract Data
```bash
python src/data_loader.py
```

### 2. Run Exploratory Analysis
```bash
jupyter notebook notebooks/01_exploratory_analysis.ipynb
```

### 3. Preprocess Data
```bash
python src/preprocessing.py
```

### 4. Feature Engineering
```bash
jupyter notebook notebooks/03_feature_engineering.ipynb
```

### 5. Train Models
```bash
python src/model_training.py
```

### 6. Generate Predictions
```bash
python src/predictions.py --input data/processed/test_data.csv
```

## 📈 Results

| Model | Accuracy | Precision | Recall | F1-Score | AUC-ROC |
|-------|----------|-----------|--------|----------|---------|
| Logistic Regression | 0.XX | 0.XX | 0.XX | 0.XX | 0.XX |
| Random Forest | 0.XX | 0.XX | 0.XX | 0.XX | 0.XX |
| Gradient Boosting | 0.XX | 0.XX | 0.XX | 0.XX | 0.XX |
| **Best Model** | **0.XX** | **0.XX** | **0.XX** | **0.XX** | **0.XX** |

### Key Performance Indicators:
- Model identifies XX% of churners correctly
- XX% precision in churn predictions
- Business ROI: [Estimated retention value]

## 🛠️ Technologies

**Data & SQL:**
- SQL (Data extraction and aggregation)
- PostgreSQL/MySQL

**Python Libraries:**
- `pandas` - Data manipulation
- `numpy` - Numerical computations
- `scikit-learn` - Machine learning
- `xgboost` - Gradient boosting
- `matplotlib`, `seaborn` - Visualization
- `sqlalchemy` - Database connection

**Tools:**
- Jupyter Notebook - Interactive analysis
- Git - Version control

## 💡 Key Findings

1. **Top Churn Drivers:**
   - [Finding 1]
   - [Finding 2]
   - [Finding 3]

2. **Customer Segments at Risk:**
   - [Segment 1]
   - [Segment 2]

3. **Retention Opportunities:**
   - [Opportunity 1]
   - [Opportunity 2]

## 🔮 Future Improvements

- [ ] Implement real-time churn scoring
- [ ] Add customer lifetime value prediction
- [ ] Develop intervention recommendation system
- [ ] Create automated ML pipeline with MLOps
- [ ] Build interactive dashboard for stakeholders
- [ ] Incorporate external data sources
- [ ] Deploy model to production

## 📞 Contact & Collaboration

For questions or suggestions, please open an issue or reach out!

---

**Last Updated:** September 2026  
**Status:** In Development
