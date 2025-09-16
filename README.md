# Heart Attack Risk Prediction

A comprehensive machine learning project that analyzes heart attack risk factors and builds predictive models using logistic regression. This project includes extensive exploratory data analysis (EDA), data preprocessing, and both custom and scikit-learn implementations of logistic regression.

## Project Overview

This project analyzes a heart attack prediction dataset containing 26 features across 8,763 patient records. The goal is to identify key risk factors and build accurate predictive models for heart attack risk assessment.

## Key Features

- **Comprehensive EDA**: Detailed analysis of 26 health and demographic variables
- **Data Preprocessing**: Outlier removal, feature engineering, and data cleaning
- **Custom ML Implementation**: Logistic regression built from scratch with regularization
- **Comparative Analysis**: Validation using scikit-learn's logistic regression
- **Geographic Analysis**: Country-wise heart attack risk assessment
- **Age Group Analysis**: Risk stratification across different age demographics

## Dataset

The dataset includes the following key variables:
- **Demographics**: Age, Sex, Country, Income
- **Health Metrics**: Cholesterol, Blood Pressure, Heart Rate, BMI, Triglycerides
- **Lifestyle Factors**: Physical Activity, Sleep Hours, Diet, Smoking
- **Medical History**: Diabetes, Family History, Previous Heart Problems
- **Target Variable**: Heart Attack Risk (Binary: 0/1)

## Methodology

### 1. Data Cleaning & Preprocessing
- Extreme outlier removal using IQR method (3×IQR bounds)
- Feature engineering (blood pressure separation, categorical encoding)
- Column renaming to camelCase convention
- Missing value analysis (dataset contains no null values)

### 2. Exploratory Data Analysis
- Correlation analysis with heart attack risk
- Geographic risk assessment across 20 countries
- Age group stratification and risk analysis
- Feature selection based on correlation strength

### 3. Machine Learning Models
- **Custom Logistic Regression**: Built from scratch with L2 regularization
- **Scikit-learn Validation**: Comparative analysis for model verification
- **Feature Selection**: Retained 12 most predictive variables

## Key Findings

### High-Impact Risk Factors
1. **Cholesterol levels** - Strong positive correlation
2. **Diabetes** - Significant risk indicator  
3. **Income** - Higher income correlates with increased risk
4. **Triglycerides** - Important metabolic marker
5. **Blood Pressure** (Systolic/Diastolic) - Classic cardiovascular indicators

### Geographic Insights
- **Highest Risk Countries**: South Korea, Nigeria, United States
- **Lowest Risk Countries**: India, Italy, Japan
- Risk variation of 8.5% across different countries

### Age Analysis
- Contrary to expectations, middle-aged groups (50-70) showed lower risk
- Suggests dataset may be biased toward high-risk populations

## Model Performance

### Custom Logistic Regression
- **Accuracy**: ~65-70%
- **F1 Score**: Balanced precision and recall
- **Regularization**: L2 penalty to prevent overfitting

### Validation Results
- Scikit-learn implementation confirms model reliability
- Consistent performance metrics across implementations

## Installation & Usage

### Prerequisites
```bash
pip install -r requirements.txt
```

### Running the Analysis
1. **Jupyter Notebook**: Open `HeartAttackPrediction.ipynb` for interactive analysis
2. **Dataset**: The notebook loads data from Google Drive (update path as needed)

### File Structure
```
├── HeartAttackPrediction.ipynb    # Main analysis notebook
├── README.md                      # Project documentation
├── requirements.txt               # Python dependencies
└── .DS_Store                      # System file (macOS)
```

### Dataset Location
The notebook expects the dataset at:
```
/content/drive/MyDrive/ds_project/heart_attack_prediction_dataset.csv
```
Update this path in the notebook to match your dataset location.

## Research Questions Addressed

1. **Predictive Accuracy**: How well can machine learning models predict heart attack risk using available features?
2. **Feature Importance**: Which variables carry the greatest weight in prediction, and what insights can be drawn?

## Data Quality Considerations

- **Sampling Bias**: Dataset shows unusual age distribution patterns
- **Geographic Representation**: 20 countries with varying sample sizes
- **Feature Reliability**: Some lifestyle factors showed counterintuitive correlations

## Future Improvements

- **Feature Engineering**: Create composite risk scores
- **Model Ensemble**: Combine multiple algorithms for better accuracy
- **Cross-validation**: Implement k-fold validation for robust evaluation
- **External Validation**: Test on independent datasets

## Additional Resources

- **Blog Post**: [Detailed EDA Analysis](https://medium.com/@writingtaha/performing-exploratory-data-analysis-eda-on-heart-risk-dataset-6f3e87e2e068)
- **Presentation Video**: [Google Drive Link](https://drive.google.com/drive/folders/1dvQlMCPBOLXsBpsnHr4GgDitxyZF9P_l?usp=share_link)

## Setup Instructions

### 1. Clone or Download
Download the project files to your local machine.

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Dataset Setup
- Download the heart attack prediction dataset
- Update the file path in `HeartAttackPrediction.ipynb` to match your dataset location
- If using Google Colab, upload the dataset to your Google Drive

### 4. Run the Analysis
Open `HeartAttackPrediction.ipynb` in Jupyter Notebook or Google Colab and run all cells.

## Contributors

Data Science Project Team

## License

This project is for educational purposes. Dataset usage should comply with original source licensing terms.

---

*Note: This analysis is for educational purposes only and should not be used for actual medical diagnosis or treatment decisions.*


## 📫 Contact & Portfolio

- **LinkedIn:** [https://www.linkedin.com/in/asfandiyar-safi-a8680b1bb/](https://www.linkedin.com/in/asfandiyar-safi-a8680b1bb/)  
- **Email:** safi.asfnd@gmail.com  
- **Portfolio / GitHub:** [https://github.com/AsfandiyarSafi](https://github.com/AsfandiyarSafi)

