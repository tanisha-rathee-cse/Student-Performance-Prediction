# Student Performance Prediction

A machine learning project to predict students' math scores using their demographic and academic details.

## Dataset
- Source: [Students Performance in Exams (Kaggle)](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams)
- 1000 rows, 8 columns (7 features + 1 target)
- Features: gender, race/ethnicity, parental level of education, lunch, test preparation course, reading score, writing score
- Target: math score

## Project Workflow
1. **Data Cleaning:** checked for null values and duplicates
2. **Exploratory Data Analysis (EDA):**
   - Heatmap (correlation between scores)
   - Box plot and violin plot (categorical vs numerical)
   - Bar plot and scatter plot
3. **Encoding:**
   - One-Hot Encoding (nominal columns)
   - Label / Ordinal Encoding (parental level of education)
   - Compared both; results were approximately the same
4. **Model Training:** Linear Regression with train-test split (75/25)
5. **Evaluation:** R² score = 87.9%

## Key Findings
- Reading and writing scores are strongly correlated with math score
- Students with standard lunch scored higher on average than those with free/reduced lunch
- Students who completed the test preparation course scored higher on average

## Tech Stack
Python, Pandas, NumPy, Matplotlib, Seaborn, scikit-learn

## Repository Structure
```
student-performance-prediction/
├── StudentsPerformance.csv
├── Student-Performance-Prediction.ipynb
├── requirements.txt
└── README.md
```

## How to Run
1. Download the notebook and `StudentsPerformance.csv` from this repo
2. Open the notebook in Jupyter or VS Code
3. Run all cells

## Future Improvements
- Try other models (Random Forest, Gradient Boosting) and compare with Linear Regression
- Add cross-validation and hyperparameter tuning
- Build a simple web app (Streamlit) for live predictions
