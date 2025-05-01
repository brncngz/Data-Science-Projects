# Data Science and Machine Learning Projects

This repository contains my various machine learning projects ranging from biological age estimation to cancer diagnosis. Each project has detailed documentation of data preprocessing, model training, and evaluation steps.

## Projects

### 1. 🔬 Biological Age Estimation from Fecal Microbiota

<img src="/api/placeholder/800/400" alt="Biological Age Estimation Image" />

**Summary:** In this project, I developed a model that estimates the biological age of individuals based on the presence of 3200 bacteria in stool samples.

**Methodology:**
- Data preprocessing and cleaning
- Visualization of age distribution
- Application of various regression models:
- Random Forest
- Gradient Boosting
- XGBoost

**Highlights:**
- Model hyperparameters were optimized using Grid Search method
- Model evaluation was performed using regression performance metrics (MAE, RMSE, R²)
- Relationship between predicted age values ​​and actual age values ​​was visualized

### 2. 🩸 Cancer Diagnosis Using Blood Microbiome Data

<img src="/api/placeholder/800/400" alt="Cancer Diagnosis Visual" />

**Summary:** In this project, I developed classification models that diagnosed four different types of cancer (colon cancer, breast cancer, lung cancer, and prostate cancer) using blood microbiome data.

**Dataset:**
- 355 patient blood samples
- 1837 features
- 4 cancer types

**Models Used:**
- Random Forest
- XGBoost
- LightGBM

**Featured Results:**
- XGBoost model 97.68% accuracy rate
- Random Forest model 95.77% accuracy rate
- Sensitivity and specificity values ​​calculated separately for each cancer type
- 100% sensitivity and precision in breast cancer and colon cancer diagnosis

## Technical Details

### Technologies Used
- Python
- Pandas (data manipulation)
- Scikit-learn (model training and evaluation)
- XGBoost, LightGBM (advanced gradient boosting libraries)
- Matplotlib/Seaborn (data visualization)

### Model Optimization
Hyperparameter optimization was performed using GridSearchCV in both projects. Optimum parameters:

**Biological Age Estimation - XGBoost:**
```python
best_params = {
'max_depth': 5,
'n_estimators': 100,
'learning_rate': 0.1
}
```

**Cancer Diagnosis - XGBoost:**
```python
best_params = {
'learning_rate': 0.1,
'max_depth': 5,
'n_estimators': 100,
'reg_alpha': 0,
'reg_lambda': 2,
'subsample': 0.8
}
```

## Installation and Running

```bash
# Clone the Repository
git clone https://github.com/username/data-science-projects.git
cd data-science-projects

# Install required libraries
pip install -r requirements.txt

# Run Jupyter Notebooks
jupyter notebook
```

## Future Work

- Implementation of deep learning models
- Improving model performance with more feature engineering
- Model generalization for different types of cancer
- More detailed analysis of microbial biomarkers

## Contact

For questions about the projects or collaboration suggestions, please contact:
- LinkedIn: [linkedin.com/in/bernacengiz](https://linkedin.com/in/bernacengiz)
