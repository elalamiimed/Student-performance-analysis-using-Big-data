# Student Performance Analysis using Big Data

A machine learning project that analyzes and predicts student academic performance based on educational behavioral data. This project leverages multiple regression and ensemble algorithms to identify key factors influencing student success.

## 📋 Overview

This project performs comprehensive analysis of student performance data, including:
- **Exploratory Data Analysis (EDA)**: Visualizes distributions across student demographics and behaviors
- **Feature Engineering**: Encodes categorical variables and identifies the most important predictors
- **Model Selection**: Compares multiple machine learning algorithms
- **Hyperparameter Tuning**: Optimizes the best-performing models
- **Ensemble Methods**: Implements advanced ensemble techniques for improved predictions

## 🎯 Key Features

- **Data Processing**: Handles categorical encoding and feature scaling
- **Feature Importance Analysis**: Identifies which student behaviors matter most
- **Multiple Algorithms**: Tests 6+ regression models including:
  - Linear Regression
  - LASSO & Elastic Net
  - K-Nearest Neighbors
  - Decision Trees
  - Support Vector Regression
  - Ensemble methods (AdaBoost, Gradient Boosting, Random Forest, Extra Trees)
- **Visualization**: Generates comparison plots and feature importance charts
- **Cross-Validation**: 10-fold cross-validation for robust model evaluation

## 📊 Dataset

The analysis uses the **xAPI-Edu-Data.csv** dataset containing 482 student records with:
- **Student Information**: Gender, nationality, grade level, section
- **Academic Engagement**: Raised hands, visited resources, announcements viewed
- **Participation**: Discussion contributions
- **Attendance**: Absence patterns
- **Parent Involvement**: Survey response and school satisfaction
- **Target Variable**: Student class (performance level)

## 🚀 Quick Start

### Prerequisites
- Python 3.x
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd Student-performance-analysis-using-Big-data
```

2. Install dependencies:
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

3. Run the analysis:
```bash
python student.py
```

The script will output:
- Dataset statistics and descriptive analysis
- Feature importance rankings
- Algorithm comparison results
- Cross-validation scores
- Final model performance metrics
- Visualization plots

## 📈 Project Workflow

1. **Data Loading & Exploration**: Load CSV and display basic statistics
2. **Data Preprocessing**: 
   - Remove irrelevant features
   - Encode categorical variables
   - Scale features for algorithms
3. **Dimensionality Reduction**: Identify and retain top 6 most important features
4. **Model Evaluation**:
   - Spot-check baseline algorithms
   - Test scaled versions with StandardScaler
   - Compare ensemble methods
5. **Hyperparameter Tuning**: 
   - Grid search for optimal LASSO alpha
   - AdaBoost estimator optimization
6. **Final Model**: Train Gradient Boosting with optimized parameters

## 📁 Project Structure

```
├── datasets.csv          # Student performance dataset
├── student.py           # Main analysis script
├── README.md            # This file
├── LICENSE              # Project license
└── R-paper.pdf          # Research paper reference
```

## 🔍 Results & Analysis

The analysis identifies which factors most strongly predict student performance:
- **Top Predictors**: VisitedResources, RaisedHands, AnnouncementsView, StudentAbsenceDays, Discussion

The best-performing model combines feature scaling with Gradient Boosting regression, achieving optimal predictions on the test set.

## 📝 Notes

- The project uses deprecated `train_test_split` from `cross_validation` module (consider updating to `model_selection`)
- All visualizations are displayed during script execution
- Results are printed to console output

## 👨‍💻 Author

Created by Dharmendra Choudhary - VIT University, Vellore, Tamil Nadu

## 📄 License

See the LICENSE file for details.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit pull requests or open issues for improvements.
