# 📞 Telco Customer Churn Prediction - Machine Learning

A comprehensive machine learning project that predicts customer churn for a telecommunications company. Using Random Forest Classification, this project helps identify customers likely to leave, enabling proactive retention strategies and reducing business losses.

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

---

## 📑 Table of Contents

- [Project Overview](#project-overview)
- [Business Problem](#business-problem)
- [Dataset Information](#dataset-information)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Data Preprocessing](#data-preprocessing)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Machine Learning Model](#machine-learning-model)
- [Model Performance](#model-performance)
- [Feature Importance](#feature-importance)
- [Key Insights](#key-insights)
- [Business Recommendations](#business-recommendations)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [Future Enhancements](#future-enhancements)
- [Contributing](#contributing)
- [Author](#author)

---

## 🎯 Project Overview

Customer churn (customer attrition) is a critical business metric for telecommunication companies. This project uses machine learning to predict which customers are likely to churn, allowing companies to take preventive action.

**Key Objectives:**
- 🎯 Predict customer churn with high accuracy
- 📊 Identify key factors driving customer attrition
- 💡 Provide actionable insights for retention
- 📈 Optimize customer lifetime value
- 💰 Reduce revenue loss from churn

**Project Impact:**
- Early identification of at-risk customers
- Targeted retention campaigns
- Improved customer satisfaction
- Reduced customer acquisition costs
- Increased profitability

---

## 💼 Business Problem

### The Challenge

**Customer Churn Costs:**
- Acquiring new customers costs 5-25x more than retaining existing ones
- Lost revenue from churned customers
- Negative word-of-mouth impact
- Decreased market share

### The Solution

**Predictive Analytics:**
- Identify at-risk customers before they churn
- Understand churn drivers
- Implement targeted retention strategies
- Optimize resource allocation for retention efforts

### Success Metrics

- **Churn Rate Reduction**: Decrease overall churn by 15-20%
- **Prediction Accuracy**: Achieve 80%+ accuracy
- **ROI**: Positive return on retention investments
- **Customer Lifetime Value**: Increase average CLV

---

## 📊 Dataset Information

### Source
**Telco Customer Churn Dataset** - IBM Sample Dataset

### Dataset Overview
- **Total Records**: 7,043 customers
- **Features**: 21 columns
- **Target Variable**: Churn (Yes/No)
- **Churn Rate**: 26.5% (1,869 churned / 5,174 retained)

### Features Description

#### Customer Demographics
| Feature | Description | Type |
|---------|-------------|------|
| **customerID** | Unique customer identifier | String |
| **gender** | Customer gender (Male/Female) | Categorical |
| **SeniorCitizen** | Whether customer is senior (1) or not (0) | Binary |
| **Partner** | Whether customer has partner (Yes/No) | Categorical |
| **Dependents** | Whether customer has dependents (Yes/No) | Categorical |

#### Account Information
| Feature | Description | Type |
|---------|-------------|------|
| **tenure** | Months customer has been with company | Numerical |
| **Contract** | Contract type (Month-to-month, One year, Two year) | Categorical |
| **PaperlessBilling** | Whether customer uses paperless billing | Categorical |
| **PaymentMethod** | Payment method used | Categorical |
| **MonthlyCharges** | Monthly bill amount | Numerical |
| **TotalCharges** | Total amount charged over tenure | Numerical |

#### Services Subscribed
| Feature | Description | Type |
|---------|-------------|------|
| **PhoneService** | Whether has phone service | Categorical |
| **MultipleLines** | Whether has multiple phone lines | Categorical |
| **InternetService** | Internet service type (DSL, Fiber optic, No) | Categorical |
| **OnlineSecurity** | Whether has online security | Categorical |
| **OnlineBackup** | Whether has online backup | Categorical |
| **DeviceProtection** | Whether has device protection | Categorical |
| **TechSupport** | Whether has tech support | Categorical |
| **StreamingTV** | Whether has streaming TV | Categorical |
| **StreamingMovies** | Whether has streaming movies | Categorical |

#### Target Variable
| Feature | Description | Values |
|---------|-------------|--------|
| **Churn** | Whether customer churned | Yes (26.5%) / No (73.5%) |

---

## ✨ Features

### Data Analysis
- ✅ **Comprehensive EDA**: In-depth exploration of 7,043+ customers
- ✅ **Churn Analysis**: Understanding attrition patterns
- ✅ **Service Analysis**: Impact of different services on churn
- ✅ **Demographic Analysis**: Age, gender, partner status effects
- ✅ **Financial Analysis**: Monthly charges and tenure correlation

### Data Preprocessing
- ✅ **Missing Value Handling**: Data quality checks
- ✅ **Data Type Conversion**: TotalCharges string to numeric
- ✅ **Categorical Encoding**: One-hot encoding for ML
- ✅ **Feature Engineering**: Creating meaningful features
- ✅ **Data Balancing**: Handling imbalanced classes

### Machine Learning
- ✅ **Random Forest Classifier**: Ensemble learning approach
- ✅ **Hyperparameter Tuning**: Optimized model parameters
- ✅ **Cross-Validation**: Robust model evaluation
- ✅ **Feature Importance**: Understanding key predictors
- ✅ **ROC-AUC Analysis**: Model performance metrics

### Visualizations
- ✅ **Churn Distribution**: Target class balance
- ✅ **Feature Importance Plot**: Top predictive features
- ✅ **ROC Curve**: Model performance visualization
- ✅ **Confusion Matrix**: Classification results
- ✅ **Service Impact Charts**: Service vs Churn analysis

---

## 🚀 Installation

### Prerequisites
- Python 3.7 or higher
- Jupyter Notebook
- pip package manager

### Step 1: Clone the Repository

```bash
git clone https://github.com/CODERGURU26/Telco-Customer-Churn-Prediction.git
cd Telco-Customer-Churn-Prediction
```

### Step 2: Install Dependencies

```bash
# Install required libraries
pip install pandas numpy matplotlib seaborn scikit-learn jupyter

# Or install all at once
pip install pandas numpy matplotlib seaborn scikit-learn jupyter imbalanced-learn
```

### Step 3: Download Dataset

The dataset is included in the repository:
- `WA_Fn-UseC_-Telco-Customer-Churn.csv`

Alternatively, download from:
- [Kaggle - Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- [IBM Sample Datasets](https://community.ibm.com/community/user/businessanalytics/blogs/steven-macko/2019/07/11/telco-customer-churn-1113)

---

## 💻 Usage

### Quick Start

1. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook
   ```

2. **Open the Project Notebook**
   ```
   Telco_Customer_Churn_-_ML.ipynb
   ```

3. **Run All Cells**
   - Execute cells sequentially
   - Train the model
   - View predictions

### Predict Customer Churn

```python
import pandas as pd
import pickle

# Load trained model (after saving)
# model = pickle.load(open('churn_model.pkl', 'rb'))

# New customer data
new_customer = {
    'gender': 'Female',
    'SeniorCitizen': 0,
    'Partner': 'Yes',
    'Dependents': 'No',
    'tenure': 12,
    'PhoneService': 'Yes',
    'MultipleLines': 'No',
    'InternetService': 'Fiber optic',
    'OnlineSecurity': 'No',
    'OnlineBackup': 'No',
    'DeviceProtection': 'No',
    'TechSupport': 'No',
    'StreamingTV': 'Yes',
    'StreamingMovies': 'Yes',
    'Contract': 'Month-to-month',
    'PaperlessBilling': 'Yes',
    'PaymentMethod': 'Electronic check',
    'MonthlyCharges': 85.00,
    'TotalCharges': 1020.00
}

# Predict churn probability
churn_probability = model.predict_proba([new_customer])
print(f"Churn Probability: {churn_probability[0][1]:.2%}")
```

---

## 🔍 Data Preprocessing

### 1. Load Data

```python
import pandas as pd

df = pd.read_csv('WA_Fn-UseC_-Telco-Customer-Churn.csv')
print(f"Dataset shape: {df.shape}")
# Output: (7043, 21)
```

### 2. Data Cleaning

```python
# Check for missing values
print(df.isnull().sum())

# Convert TotalCharges to numeric (it's string type)
df['TotalCharges'] = pd.to_numeric(df['TotalCharges'], errors='coerce')

# Fill missing values (11 rows have empty TotalCharges)
df['TotalCharges'].fillna(df['TotalCharges'].median(), inplace=True)

# Verify no missing values
print(f"Missing values: {df.isnull().sum().sum()}")
```

### 3. Handle Target Variable

```python
# Convert Churn to binary
df['Churn'] = df['Churn'].map({'Yes': 1, 'No': 0})

# Check distribution
print(df['Churn'].value_counts())
# 0 (No Churn):  5174 (73.5%)
# 1 (Churn):     1869 (26.5%)
```

### 4. Encode Categorical Variables

```python
# Method 1: One-Hot Encoding
df_encoded = pd.get_dummies(df, drop_first=True)

# Method 2: Label Encoding (for tree-based models)
from sklearn.preprocessing import LabelEncoder

categorical_cols = df.select_dtypes(include=['object']).columns
le = LabelEncoder()

for col in categorical_cols:
    if col != 'customerID':
        df[col] = le.fit_transform(df[col])

# Drop customerID (not predictive)
df = df.drop('customerID', axis=1)
```

### 5. Feature Engineering

```python
# Create tenure groups
df['tenure_group'] = pd.cut(df['tenure'], 
                             bins=[0, 12, 24, 48, 72],
                             labels=['0-1 year', '1-2 years', '2-4 years', '4+ years'])

# Calculate average monthly charge
df['avg_monthly_charge'] = df['TotalCharges'] / (df['tenure'] + 1)

# Create service count feature
service_cols = ['PhoneService', 'InternetService', 'OnlineSecurity', 
                'OnlineBackup', 'DeviceProtection', 'TechSupport', 
                'StreamingTV', 'StreamingMovies']
df['num_services'] = df[service_cols].apply(lambda x: x.str.contains('Yes').sum(), axis=1)
```

---

## 📊 Exploratory Data Analysis

### Churn Distribution

```python
import matplotlib.pyplot as plt
import seaborn as sns

# Churn count
plt.figure(figsize=(8, 6))
df['Churn'].value_counts().plot(kind='bar', color=['green', 'red'])
plt.title('Customer Churn Distribution', fontsize=16)
plt.xlabel('Churn Status (0=No, 1=Yes)', fontsize=12)
plt.ylabel('Count', fontsize=12)
plt.xticks(rotation=0)
plt.show()

# Churn percentage
churn_rate = df['Churn'].mean() * 100
print(f"Overall Churn Rate: {churn_rate:.2f}%")
```

### Churn by Contract Type

```python
plt.figure(figsize=(10, 6))
pd.crosstab(df['Contract'], df['Churn'], normalize='index').plot(kind='bar', stacked=True)
plt.title('Churn Rate by Contract Type', fontsize=16)
plt.xlabel('Contract Type', fontsize=12)
plt.ylabel('Proportion', fontsize=12)
plt.legend(['Retained', 'Churned'])
plt.xticks(rotation=45)
plt.show()
```

### Churn by Tenure

```python
plt.figure(figsize=(12, 6))
sns.histplot(data=df, x='tenure', hue='Churn', bins=30, kde=True)
plt.title('Customer Tenure Distribution by Churn Status', fontsize=16)
plt.xlabel('Tenure (months)', fontsize=12)
plt.ylabel('Count', fontsize=12)
plt.show()
```

### Monthly Charges vs Churn

```python
plt.figure(figsize=(10, 6))
sns.boxplot(data=df, x='Churn', y='MonthlyCharges')
plt.title('Monthly Charges Distribution by Churn Status', fontsize=16)
plt.xlabel('Churn (0=No, 1=Yes)', fontsize=12)
plt.ylabel('Monthly Charges ($)', fontsize=12)
plt.show()
```

### Service Impact on Churn

```python
# Services analysis
services = ['OnlineSecurity', 'OnlineBackup', 'DeviceProtection', 
            'TechSupport', 'StreamingTV', 'StreamingMovies']

fig, axes = plt.subplots(2, 3, figsize=(15, 10))
axes = axes.ravel()

for idx, service in enumerate(services):
    pd.crosstab(df[service], df['Churn'], normalize='index').plot(
        kind='bar', ax=axes[idx], legend=False
    )
    axes[idx].set_title(f'{service} vs Churn')
    axes[idx].set_xlabel('')

plt.tight_layout()
plt.show()
```

### Correlation Heatmap

```python
plt.figure(figsize=(12, 10))
correlation = df.corr()
sns.heatmap(correlation, annot=False, cmap='coolwarm', center=0)
plt.title('Feature Correlation Heatmap', fontsize=16)
plt.tight_layout()
plt.show()

# Top correlations with Churn
churn_corr = correlation['Churn'].sort_values(ascending=False)
print("Top Correlations with Churn:")
print(churn_corr.head(10))
```

---

## 🤖 Machine Learning Model

### Model Selection: Random Forest Classifier

**Why Random Forest?**
- ✅ Handles non-linear relationships
- ✅ Robust to outliers
- ✅ Provides feature importance
- ✅ Good with imbalanced data
- ✅ Excellent for tabular data

### Complete ML Pipeline

#### 1. Split Features and Target

```python
from sklearn.model_selection import train_test_split

# Separate features and target
X = df.drop('Churn', axis=1)
y = df['Churn']

print(f"Features shape: {X.shape}")
print(f"Target shape: {y.shape}")
```

#### 2. Train-Test Split

```python
X_train, X_test, y_train, y_test = train_test_split(
    X, y, 
    test_size=0.2,      # 80-20 split
    random_state=42,    # Reproducibility
    stratify=y          # Maintain class distribution
)

print(f"Training set: {X_train.shape[0]} samples")
print(f"Test set: {X_test.shape[0]} samples")
print(f"Train churn rate: {y_train.mean():.2%}")
print(f"Test churn rate: {y_test.mean():.2%}")
```

#### 3. Handle Class Imbalance (Optional)

```python
from imblearn.over_sampling import SMOTE

# Apply SMOTE
smote = SMOTE(random_state=42)
X_train_balanced, y_train_balanced = smote.fit_resample(X_train, y_train)

print(f"Original training set: {y_train.value_counts()}")
print(f"Balanced training set: {y_train_balanced.value_counts()}")
```

#### 4. Model Training - Basic

```python
from sklearn.ensemble import RandomForestClassifier

# Initialize model
model = RandomForestClassifier(
    n_estimators=100,    # Number of trees
    random_state=42
)

# Train model
model.fit(X_train, y_train)
print("Model training completed!")
```

#### 5. Model Training - Optimized

```python
# Optimized hyperparameters
model = RandomForestClassifier(
    n_estimators=200,        # More trees
    max_depth=10,            # Prevent overfitting
    min_samples_split=10,    # Minimum samples to split
    min_samples_leaf=5,      # Minimum samples in leaf
    max_features='sqrt',     # Features per split
    random_state=42,
    n_jobs=-1               # Use all CPU cores
)

# Train model
model.fit(X_train, y_train)
```

#### 6. Model Training - Grid Search

```python
from sklearn.model_selection import GridSearchCV

# Define parameter grid
param_grid = {
    'n_estimators': [100, 200, 300],
    'max_depth': [5, 10, 15, None],
    'min_samples_split': [2, 5, 10],
    'min_samples_leaf': [1, 2, 5]
}

# Grid search
grid_search = GridSearchCV(
    RandomForestClassifier(random_state=42),
    param_grid,
    cv=5,
    scoring='roc_auc',
    n_jobs=-1,
    verbose=1
)

grid_search.fit(X_train, y_train)
print(f"Best parameters: {grid_search.best_params_}")
print(f"Best ROC-AUC score: {grid_search.best_score_:.4f}")

# Use best model
model = grid_search.best_estimator_
```

#### 7. Make Predictions

```python
# Predict on test set
y_pred = model.predict(X_test)

# Predict probabilities
y_pred_proba = model.predict_proba(X_test)[:, 1]

# Sample predictions
print("Sample Predictions:")
results = pd.DataFrame({
    'Actual': y_test[:10].values,
    'Predicted': y_pred[:10],
    'Probability': y_pred_proba[:10]
})
print(results)
```

---

## 📈 Model Performance

### Evaluation Metrics

```python
from sklearn.metrics import (
    accuracy_score, precision_score, recall_score, f1_score,
    confusion_matrix, classification_report, roc_auc_score, roc_curve
)

# Calculate metrics
accuracy = accuracy_score(y_test, y_pred)
precision = precision_score(y_test, y_pred)
recall = recall_score(y_test, y_pred)
f1 = f1_score(y_test, y_pred)
roc_auc = roc_auc_score(y_test, y_pred_proba)

print("Model Performance Metrics:")
print(f"Accuracy:  {accuracy:.4f} ({accuracy*100:.2f}%)")
print(f"Precision: {precision:.4f}")
print(f"Recall:    {recall:.4f}")
print(f"F1-Score:  {f1:.4f}")
print(f"ROC-AUC:   {roc_auc:.4f}")
```

### Expected Results

| Metric | Score | Interpretation |
|--------|-------|----------------|
| **Accuracy** | ~79-83% | Overall correctness |
| **Precision** | ~65-70% | Accuracy of churn predictions |
| **Recall** | ~50-60% | Coverage of actual churners |
| **F1-Score** | ~60-65% | Balanced performance |
| **ROC-AUC** | ~82-85% | Model discriminative ability |

### Train vs Test Accuracy

```python
train_accuracy = model.score(X_train, y_train)
test_accuracy = model.score(X_test, y_test)

print(f"Train Accuracy: {train_accuracy:.4f}")
print(f"Test Accuracy:  {test_accuracy:.4f}")
print(f"Difference:     {abs(train_accuracy - test_accuracy):.4f}")

if train_accuracy - test_accuracy > 0.05:
    print("⚠️ Model may be overfitting!")
else:
    print("✓ Model generalizes well!")
```

### Confusion Matrix

```python
import seaborn as sns
import matplotlib.pyplot as plt

# Calculate confusion matrix
cm = confusion_matrix(y_test, y_pred)

# Visualize
plt.figure(figsize=(8, 6))
sns.heatmap(cm, annot=True, fmt='d', cmap='Blues', cbar=False)
plt.title('Confusion Matrix', fontsize=16)
plt.ylabel('Actual', fontsize=12)
plt.xlabel('Predicted', fontsize=12)
plt.xticks([0.5, 1.5], ['No Churn', 'Churn'])
plt.yticks([0.5, 1.5], ['No Churn', 'Churn'])
plt.show()

# Breakdown
tn, fp, fn, tp = cm.ravel()
print(f"True Negatives:  {tn}")
print(f"False Positives: {fp}")
print(f"False Negatives: {fn}")
print(f"True Positives:  {tp}")
```

### Classification Report

```python
print("\nDetailed Classification Report:")
print(classification_report(y_test, y_pred, 
                            target_names=['No Churn', 'Churn']))
```

### ROC Curve

```python
from sklearn.metrics import roc_curve, auc

# Calculate ROC curve
fpr, tpr, thresholds = roc_curve(y_test, y_pred_proba)
roc_auc = auc(fpr, tpr)

# Plot
plt.figure(figsize=(10, 8))
plt.plot(fpr, tpr, color='darkorange', lw=2, 
         label=f'ROC Curve (AUC = {roc_auc:.2f})')
plt.plot([0, 1], [0, 1], color='navy', lw=2, linestyle='--', 
         label='Random Classifier')
plt.xlim([0.0, 1.0])
plt.ylim([0.0, 1.05])
plt.xlabel('False Positive Rate', fontsize=12)
plt.ylabel('True Positive Rate', fontsize=12)
plt.title('Receiver Operating Characteristic (ROC) Curve', fontsize=16)
plt.legend(loc="lower right")
plt.grid(True, alpha=0.3)
plt.show()
```

---

## 🎯 Feature Importance

### Extract Feature Importance

```python
import pandas as pd

# Get feature importances
importance = pd.Series(
    model.feature_importances_,
    index=X.columns
).sort_values(ascending=False)

# Display top features
print("Top 10 Most Important Features:")
print(importance.head(10))
```

### Visualize Feature Importance

```python
# Top 10 features
plt.figure(figsize=(12, 8))
importance.head(10).plot(kind='barh', color='steelblue')
plt.title('Top 10 Feature Importance', fontsize=16)
plt.xlabel('Importance Score', fontsize=12)
plt.ylabel('Features', fontsize=12)
plt.gca().invert_yaxis()
plt.tight_layout()
plt.show()
```

### Expected Top Features

Based on typical telco churn analysis:

1. **Tenure** (30-35%): Longest-staying customers less likely to churn
2. **Contract** (20-25%): Month-to-month contracts higher churn
3. **MonthlyCharges** (15-20%): Higher charges correlate with churn
4. **TotalCharges** (10-15%): Total spend indicator
5. **InternetService** (8-12%): Service type impacts churn
6. **TechSupport** (5-8%): Lack of support increases churn
7. **OnlineSecurity** (4-6%): Security features reduce churn
8. **PaymentMethod** (3-5%): Payment method influences churn
9. **PaperlessBilling** (2-4%): Billing method impact
10. **SeniorCitizen** (1-3%): Age demographic factor

---

## 💡 Key Insights

### Customer Behavior Patterns

1. **Contract Type is Critical**
   - Month-to-month contracts: ~42% churn rate
   - One-year contracts: ~11% churn rate
   - Two-year contracts: ~3% churn rate
   - **Insight**: Long-term contracts dramatically reduce churn

2. **New Customers at High Risk**
   - Customers with tenure < 6 months: 50%+ churn rate
   - Customers with tenure > 24 months: < 10% churn rate
   - **Insight**: First 6 months are critical retention period

3. **Price Sensitivity**
   - Churned customers have 15-20% higher monthly charges
   - Average churned: $75/month
   - Average retained: $62/month
   - **Insight**: Pricing directly impacts retention

4. **Service Bundle Effect**
   - Customers with 0-1 services: 40% churn rate
   - Customers with 4+ services: 15% churn rate
   - **Insight**: Service bundling increases stickiness

5. **Support Services Matter**
   - No tech support: 41% churn rate
   - With tech support: 15% churn rate
   - No online security: 42% churn rate
   - With online security: 15% churn rate
   - **Insight**: Support services significantly reduce churn

6. **Payment Method Impact**
   - Electronic check: 45% churn rate
   - Bank transfer: 17% churn rate
   - Credit card: 15% churn rate
   - **Insight**: Payment method indicates customer commitment

### Demographic Insights

```python
# Senior citizens
senior_churn = df[df['SeniorCitizen'] == 1]['Churn'].mean()
non_senior_churn = df[df['SeniorCitizen'] == 0]['Churn'].mean()
print(f"Senior citizen churn rate: {senior_churn:.2%}")
print(f"Non-senior churn rate: {non_senior_churn:.2%}")

# Partner status
partner_churn = df[df['Partner'] == 'Yes']['Churn'].mean()
no_partner_churn = df[df['Partner'] == 'No']['Churn'].mean()
print(f"With partner churn rate: {partner_churn:.2%}")
print(f"Without partner churn rate: {no_partner_churn:.2%}")
```

---

## 💼 Business Recommendations

### 1. **Retention Strategy for New Customers**

**Problem**: High churn in first 6 months

**Solutions:**
- Enhanced onboarding program
- Dedicated account manager for first 90 days
- Welcome package with service tutorials
- Monthly check-in calls
- Special new customer discount

**Expected Impact**: 15-20% reduction in early churn

---

### 2. **Contract Type Incentives**

**Problem**: Month-to-month contracts have 40%+ churn

**Solutions:**
- Offer 10-15% discount for annual contracts
- Provide contract upgrade bonuses
- Highlight long-term value proposition
- Create loyalty rewards for contract renewals
- Bundle services with contract commitments

**Expected Impact**: 20-25% conversion to longer contracts

---

### 3. **Service Bundle Optimization**

**Problem**: Single-service customers at high risk

**Solutions:**
- Personalized bundle recommendations
- Cross-sell campaigns based on usage
- Bundle discount packages
- Free trial periods for additional services
- Gamification for service adoption

**Expected Impact**: 30% increase in multi-service adoption

---

### 4. **Pricing Strategy**

**Problem**: High monthly charges correlate with churn

**Solutions:**
- Value-based pricing tiers
- Loyalty discounts for long-tenure customers
- Competitive price matching program
- Transparent pricing with no hidden fees
- Flexible payment plans

**Expected Impact**: 10-15% churn reduction

---

### 5. **Support Service Enhancement**

**Problem**: Lack of tech support drives churn

**Solutions:**
- Include basic tech support for all customers
- 24/7 support availability
- Proactive outreach for service issues
- Self-service knowledge base
- Premium support tier option

**Expected Impact**: 18-22% churn reduction

---

### 6. **Payment Method Optimization**

**Problem**: Electronic check users churn more

**Solutions:**
- Incentivize automatic payment enrollment
- Offer payment method bonuses
- Simplify payment change process
- Provide payment flexibility options
- Reward automatic payments with perks

**Expected Impact**: 8-10% improvement in retention

---

### 7. **Targeted Retention Campaigns**

**Use ML Model Predictions:**

```python
# Identify high-risk customers
high_risk_threshold = 0.7
high_risk_customers = df[df['churn_probability'] > high_risk_threshold]

# Segment by risk level
segments = pd.cut(df['churn_probability'], 
                  bins=[0, 0.3, 0.7, 1.0],
                  labels=['Low Risk', 'Medium Risk', 'High Risk'])

# Targeted interventions
for segment in segments.unique():
    segment_customers = df[segments == segment]
    print(f"\n{segment}: {len(segment_customers)} customers")
    # Apply appropriate retention strategy
```

**Campaign Tiers:**
- **Low Risk (< 30%)**: Loyalty rewards, upsell opportunities
- **Medium Risk (30-70%)**: Personalized offers, service upgrades
- **High Risk (> 70%)**: Aggressive retention, win-back campaigns

---

## 🛠️ Technologies Used

### Core Technologies

| Technology | Purpose | Version |
|------------|---------|---------|
| **Python** | Programming language | 3.7+ |
| **Pandas** | Data manipulation | Latest |
| **NumPy** | Numerical computing | Latest |
| **Scikit-learn** | Machine learning | Latest |
| **Matplotlib** | Visualization | Latest |
| **Seaborn** | Statistical visualization | Latest |
| **Jupyter** | Interactive development | Latest |

### Libraries & Functions

```python
# Data Processing
import pandas as pd
import numpy as np

# Machine Learning
from sklearn.model_selection import train_test_split, GridSearchCV, cross_val_score
from sklearn.ensemble import RandomForestClassifier
from sklearn.metrics import (accuracy_score, precision_score, recall_score, 
                             f1_score, confusion_matrix, classification_report,
                             roc_auc_score, roc_curve, auc)

# Visualization
import matplotlib.pyplot as plt
import seaborn as sns

# Class Imbalance
from imblearn.over_sampling import SMOTE

# Model Persistence
import pickle
```

---

## 📂 Project Structure

```
Telco-Customer-Churn-Prediction/
│
├── Telco_Customer_Churn_-_ML.ipynb
│   └── Main analysis and ML notebook
│
├── WA_Fn-UseC_-Telco-Customer-Churn.csv
│   └── Dataset (7,043 customers)
│
├── models/
│   ├── churn_model.pkl
│   └── scaler.pkl
│
├── visualizations/
│   ├── churn_distribution.png
│   ├── feature_importance.png
│   ├── roc_curve.png
│   └── confusion_matrix.png
│
├── requirements.txt
│   └── Python dependencies
│
└── README.md
    └── Project documentation (this file)
```

---

## 🔮 Future Enhancements

### Model Improvements
- [ ] Try XGBoost and LightGBM
- [ ] Implement deep learning models
- [ ] Ensemble multiple models
- [ ] Add SHAP for explainability
- [ ] Time series churn prediction
- [ ] Customer lifetime value prediction

### Feature Engineering
- [ ] RFM (Recency, Frequency, Monetary) analysis
- [ ] Customer segmentation clustering
- [ ] Interaction features
- [ ] Temporal features (seasonality)
- [ ] Network effects (referrals)
- [ ] Usage pattern features

### Deployment
- [ ] Create Flask API for predictions
- [ ] Build Streamlit dashboard
- [ ] Deploy on AWS/Heroku
- [ ] Real-time prediction pipeline
- [ ] Automated retraining pipeline
- [ ] A/B testing framework

### Business Intelligence
- [ ] Interactive Power BI dashboard
- [ ] Automated email reports
- [ ] Customer risk scoring system
- [ ] Campaign ROI calculator
- [ ] Churn prevention cost analysis
- [ ] Customer segmentation tool

---

## 🐛 Troubleshooting

### Common Issues

#### Issue 1: TotalCharges Data Type Error
**Error:** `ValueError: could not convert string to float`

**Solution:**
```python
# TotalCharges has spaces for new customers
df['TotalCharges'] = pd.to_numeric(df['TotalCharges'], errors='coerce')
df['TotalCharges'].fillna(df['TotalCharges'].median(), inplace=True)
```

#### Issue 2: Imbalanced Classes
**Problem:** Model predicts all customers as "No Churn"

**Solution:**
```python
# Use SMOTE or class weights
from imblearn.over_sampling import SMOTE

smote = SMOTE(random_state=42)
X_train_balanced, y_train_balanced = smote.fit_resample(X_train, y_train)

# Or use class weights in model
model = RandomForestClassifier(class_weight='balanced')
```

#### Issue 3: Low Recall
**Problem:** Model misses many churners (high false negatives)

**Solution:**
```python
# Adjust prediction threshold
threshold = 0.3  # Lower than default 0.5
y_pred_adjusted = (y_pred_proba > threshold).astype(int)

# Or use different evaluation metric
from sklearn.model_selection import cross_val_score
scores = cross_val_score(model, X, y, cv=5, scoring='recall')
```

#### Issue 4: Feature Encoding Issues
**Problem:** Too many features after one-hot encoding

**Solution:**
```python
# Use drop_first to avoid dummy variable trap
df_encoded = pd.get_dummies(df, drop_first=True)

# Or use target encoding for high-cardinality features
from category_encoders import TargetEncoder
encoder = TargetEncoder()
df['PaymentMethod_encoded'] = encoder.fit_transform(
    df['PaymentMethod'], df['Churn']
)
```

---

## 🎓 Learning Outcomes

This project demonstrates:

- ✅ **Binary Classification**: Predicting binary outcomes
- ✅ **Imbalanced Data Handling**: Working with skewed classes
- ✅ **Feature Engineering**: Creating predictive features
- ✅ **Model Evaluation**: Using multiple metrics
- ✅ **Business Analytics**: Translating data to insights
- ✅ **Random Forest**: Ensemble learning
- ✅ **ROC-AUC Analysis**: Model performance assessment
- ✅ **Feature Importance**: Understanding drivers

---

## 🤝 Contributing

Contributions welcome! Ways to contribute:

1. **Fork the repository**
2. **Create feature branch**
   ```bash
   git checkout -b feature/NewFeature
   ```
3. **Make improvements**
   - Add new models
   - Improve visualizations
   - Enhance documentation
4. **Commit and push**
   ```bash
   git commit -m 'Add: New feature'
   git push origin feature/NewFeature
   ```
5. **Open Pull Request**

### Contribution Ideas
- Implement gradient boosting models
- Add SHAP explainability
- Create web dashboard
- Build API endpoint
- Add customer segmentation
- Implement A/B testing framework

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

**Dataset License**: IBM Sample Dataset for educational purposes.

---

## 📧 Contact & Connect

### Author

**Gururaj Krishna Sharma**

- 📧 Email: [guruuu2468@gmail.com](mailto:guruuu2468@gmail.com)
- 💼 LinkedIn: [Gururaj Krishna Sharma](https://www.linkedin.com/in/gururaj-krishna-sharma)
- 💻 GitHub: [@CODERGURU26](https://github.com/CODERGURU26)

---

## 🌟 Acknowledgments

- **IBM** for providing the sample dataset
- **Scikit-learn** team for excellent ML tools
- **Kaggle** community for dataset hosting
- **Telco industry** for inspiring this analysis
- **Data science community** for best practices

---

## 📚 Additional Resources

### Learn More
- [Scikit-learn Documentation](https://scikit-learn.org/stable/)
- [Random Forest Explained](https://www.stat.berkeley.edu/~breiman/RandomForests/)
- [Imbalanced Learn](https://imbalanced-learn.org/)
- [Customer Churn Analysis Guide](https://www.profitwell.com/customer-churn/analysis)

### Related Projects
- Credit card fraud detection
- Customer lifetime value prediction
- Marketing campaign optimization
- Loan default prediction

---

## 🎯 Business Impact

**For Telecom Companies:**
- Reduce customer acquisition costs
- Increase customer lifetime value
- Improve retention rates
- Optimize marketing spend
- Enhance customer satisfaction

**For Data Scientists:**
- Learn classification techniques
- Practice feature engineering
- Build portfolio project
- Understand business applications

**For Business Analysts:**
- Data-driven decision making
- Customer behavior insights
- ROI calculation
- Strategic planning

---

**⭐ If you find this project helpful, please give it a star!**

**🔔 Watch this repository for updates!**

---

*Last Updated: February 2026*

**Happy Analyzing! 📊📞**

**Remember:** The goal isn't just prediction—it's retention! 💡
