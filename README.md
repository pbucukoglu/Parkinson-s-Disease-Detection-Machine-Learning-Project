# Parkinson’s Disease Detection with Machine Learning

This project focuses on the early diagnosis of Parkinson’s Disease using various machine learning models. The dataset includes biomedical voice measurements from people with and without Parkinson's Disease.

## 📁 Project Structure

```
├── Parkinsons_Final.ipynb         # Main Jupyter notebook
├── parkinsons_disease_data.csv    # Dataset
├── FinalReport.pdf                # IEEE-format final report
└── README.md                      # Project overview
```

## 🧠 Objective

To develop and compare machine learning models that can accurately classify whether a person has Parkinson’s Disease based on vocal features.

## 📊 Dataset

- **Samples:** 195 instances
- **Features:** 23 biomedical voice measurements (e.g., MDVP:Fo(Hz), MDVP:Jitter(%), etc.)
- **Target:** `status` (1 = Parkinson’s, 0 = healthy)

## 🧹 Data Preprocessing

- Handled missing and outlier values
- Scaled features for consistency
- Applied **SMOTE** to handle class imbalance

## 🔍 Exploratory Data Analysis (EDA)

- Correlation heatmaps
- Distribution plots of key features
- Class imbalance visualization

## 🤖 Models Used

| Model               | Description                          |
|--------------------|--------------------------------------|
| Logistic Regression| Baseline linear classifier           |
| SVM                | Support Vector Machine with kernels  |
| KNN                | K-Nearest Neighbors                  |
| Decision Tree      | Tree-based classification            |
| Random Forest      | Ensemble of decision trees           |
| Voting Classifier  | Combines top-performing models       |

## 🎯 Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

## 🏆 Results

- The **Voting Classifier** (ensemble of SVM, KNN, and Random Forest) achieved the best results.
- **SMOTE** significantly improved model performance by balancing the dataset.

## 📄 Final Report

The full analysis and methodology can be found in the included PDF file: [`FinalReport.pdf`](./FinalReport.pdf)

## 📚 Requirements

- Python 3.7+
- pandas
- numpy
- scikit-learn
- seaborn
- matplotlib
- imbalanced-learn

