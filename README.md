# Data Science Fundamentals Assessment

Assessment submission for **Yuva Intern** covering core data science fundamentals: Python basics, data types, data cleaning, statistical foundations, and industry best practices.

**Author:** Rajat ([GitHub](https://github.com/rajatmaurya) | [LinkedIn](https://linkedin.com/in/rajatmaurya) | [Kaggle](https://kaggle.com/rajatmaurya))

## What's inside

| File | Description |
|---|---|
| `Data_Science_Fundamentals.ipynb` | Jupyter notebook with all code, explanations and visualisations |
| `Data_Science_Fundamentals_Report.docx` | Written report submitted to the platform |
| `README.md` | Project overview (this file) |

## Topics covered

1. **Python basics**: variables, collections (list, tuple, set, dict), control flow, functions, list comprehensions, NumPy arrays
2. **Data types**: quantitative (discrete, continuous) and qualitative (nominal, ordinal); Pandas dtypes and categorical conversion
3. **Data cleaning**: missing values, duplicates, median imputation
4. **Descriptive statistics**: mean, median, mode, standard deviation, variance, quartiles, IQR, skewness
5. **Outlier detection**: 1.5 x IQR rule
6. **Visualisation**: histogram, boxplot, correlation heatmap, regression plot
7. **Inferential statistics**: Pearson correlation test, two-sample t-test, simple linear regression
8. **Best practices**: reproducibility, version control, clean code, avoiding data leakage, right metrics, ethics

## Dataset

A small synthetic dataset of 10 students, created inside the notebook:

| Column | Type | Description |
|---|---|---|
| `student_id` | int | Unique ID |
| `hours_studied` | int | Study hours |
| `attendance_pct` | int | Attendance percentage |
| `gender` | category | M / F |
| `score` | float | Exam score (one value deliberately missing to practise cleaning) |

## Key findings

- Mean score is 69.2 and median is 70.0, so the distribution is roughly symmetric (skewness about 0.03).
- No outliers under the 1.5 x IQR rule.
- Hours studied vs score: **r = 0.979, p < 0.05**, a very strong and statistically significant positive relationship.
- The gender difference in scores is not statistically significant in this sample.

**Limitations:** only 10 observations, and correlation does not imply causation. Hours studied and attendance are also highly correlated with each other (multicollinearity).

## How to run

```bash
# 1. Clone the repo
git clone https://github.com/rajatcse9-a11y/DS_Fundametal_Project.git
cd DS_Fundametal_Project

# 2. (Optional) create a virtual environment
python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate

# 3. Install dependencies
pip install numpy pandas matplotlib scipy jupyter

# 4. Launch the notebook
jupyter notebook Data_Science_Fundamentals.ipynb
```

You can also upload the notebook to [Google Colab](https://colab.research.google.com) and use **Runtime > Run all**. No extra setup is needed there.

## Tech stack

Python 3 | NumPy | Pandas | Matplotlib | SciPy | Jupyter

## License

This project is for educational purposes.