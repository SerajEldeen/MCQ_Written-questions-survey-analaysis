# Phase Six: Data Analysis Plan

## Overview

This phase focuses on analyzing survey data related to student preferences and experiences with different examination systems (MCQ vs Written). The analysis will be conducted using two main tools:

- **Power BI** → for descriptive analysis and visualization
- **Python (Jupyter Notebook)** → for statistical testing and predictive modeling

---

# 1. Data Preparation

Before analysis, the dataset will be cleaned and transformed:

## Data Transformation

- Group open-ended responses:
  - Field of Study → (Engineering, Business, Medical, etc.)
  - Perfect Exam System → (MCQ, Written, Projects, Mixed)

## Encoding

- Create numerical versions of categorical columns:
  - Gender → Male=1, Female=0
  - Level → High School=0, Undergraduate=1, Postgraduate=2
  - Age → Under 18=0, 18–22=1, 23–28=2
  - Exam Frequency → Rarely=0, Sometimes=1, Very Often=2
  - Exam Type (Stress/Preference) → MCQ=0, Written=1, Both=2

- Likert Scale Questions remain numeric:
  - 1 = Strongly Disagree
  - 5 = Strongly Agree

---

# 2. Power BI Analysis

Power BI will be used for **Descriptive Statistics, Correlation Exploration, and Visualization**.

## A. Descriptive Statistics

- Calculate:
  - Mean (e.g., average stress level)
  - Counts (e.g., number of students by gender)
  - Frequency distributions (MCQ vs Written preference)

## B. Data Visualization

The analysis results in a comprehensive dashboard that tracks student sentiment and academic trends.

![Student Examination Stress Dashboard](./Dashboard.png)

- Preparation difficulty vs performance perception

---

# 3. Python Analysis (Jupyter Notebook)

Python will be used for **Inferential Statistics and Regression Analysis**.

## A. Correlation Analysis

- Compute correlation matrix
- Identify strength and direction of relationships between variables

Example:

- Stress vs Time Pressure
- MCQ fairness vs knowledge reflection

---

## B. Inferential Statistics

### 1. T-Test

- Compare means between two groups

Example:

- Stress level in MCQ vs Written exams

Goal:

- Determine if difference is statistically significant

---

### 2. Chi-Square Test

- Test relationships between categorical variables

Example:

- Gender vs Exam Preference

Goal:

- Check dependency between variables

---

## C. Regression Analysis

Build a predictive model:

### Target Variable:

- Written Exam Stress

### Features (Independent Variables):

- Time Pressure
- MCQ Ease of Preparation
- Exam Frequency
- Perceived Fairness

### Purpose:

- Understand which factors most influence student stress

---

# 4. Interpretation & Reporting

## The final results will be documented in a Word report.

# 5. Final Workflow

1. Clean and preprocess data (Python)
2. Create structured dataset
3. Import into Power BI → build dashboard
4. Export dataset → analyze in Python
5. Perform statistical tests and regression
6. Write final report with insights and conclusions

---

# Outcome

By the end of this phase, the project will include:

- Interactive Power BI Dashboard
- Python Notebook with statistical analysis
- Written report with clear interpretations and conclusions
