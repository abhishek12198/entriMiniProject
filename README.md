# ABC Company Employee Data Analysis Project

## Project Overview

This project focuses on analyzing employee data from ABC Company using Python in Google Colab. The dataset contains 458 rows and 9 columns, providing information about employees, including their teams, positions, age, salary, and height.

The objective of the project is to preprocess the dataset, perform data analysis, generate graphical visualizations, and derive meaningful business insights from the employee data.

---

# Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib

---

# Dataset Information

The dataset consists of:
- 458 employee records
- 9 columns containing employee-related information

Key columns used in analysis:
- Name
- Team
- Position
- Age
- Salary
- Height

---

# Preprocessing Steps

## Height Column Correction

The dataset contained inconsistent values in the `height` column. To ensure consistency and maintain data integrity, the height values were replaced with randomly generated numbers between 150 cm and 180 cm.

### Preprocessing Code

```python
import random

df['height'] = [random.randint(150, 180) for _ in range(len(df))]
```

This preprocessing step ensured:
- Uniform data formatting
- Valid height ranges
- Improved reliability for further analysis

---

# Analysis Tasks Performed

## 1. Employee Distribution Across Teams

The total number of employees in each team was calculated along with the percentage contribution relative to the total workforce.

### Objectives
- Understand workforce allocation
- Identify larger and smaller teams

### Visualization Used
- Pie Chart
- Bar Chart

---

## 2. Employee Segregation Based on Positions

Employees were grouped according to their job positions within the organization.

### Objectives
- Identify dominant job roles
- Analyze organizational structure

### Visualization Used
- Bar Chart

---

## 3. Predominant Age Group Analysis

Employees were categorized into different age groups to determine the most common age category.

### Objectives
- Understand workforce demographics
- Analyze employee age distribution

### Visualization Used
- Bar Chart

---

## 4. Salary Expenditure Analysis

Salary expenses were analyzed based on:
- Teams
- Positions

The team and position with the highest salary expenditure were identified.

### Objectives
- Analyze payroll distribution
- Identify high-cost departments and roles

### Visualization Used
- Horizontal Bar Charts

---

## 5. Correlation Between Age and Salary

A correlation analysis was conducted to examine the relationship between employee age and salary.

### Objectives
- Determine whether salary increases with age and experience
- Identify trends in compensation

### Visualization Used
- Scatter Plot
- Trend Line Graph

---

# Key Insights and Findings

## Workforce Distribution
Some teams contain a significantly larger number of employees, indicating higher operational demands in those departments.

## Position Analysis
A few positions dominate the workforce, showing that certain roles are essential for the organization’s daily operations.

## Age Demographics
Most employees belong to middle-age groups, suggesting a balanced workforce with adequate experience and productivity.

## Salary Trends
Specific teams and positions contribute heavily to total salary expenditure, reflecting leadership and specialized responsibilities.

## Age vs Salary Correlation
The correlation analysis indicates a moderate positive relationship between age and salary, suggesting that employee compensation tends to increase with experience.

---

# Graphical Representations Included

The project contains the following visualizations:

1. Team-wise employee distribution chart
2. Position-wise employee count chart
3. Age group distribution graph
4. Team-wise salary expenditure graph
5. Position-wise salary expenditure graph
6. Age vs Salary scatter plot with trend line

These visualizations help present the findings in a clear and interactive manner.

---

# Conclusion

This project successfully demonstrates how employee datasets can be preprocessed, analyzed, and visualized using Python tools. The analysis provides valuable insights into workforce distribution, salary allocation, employee demographics, and organizational structure.

The findings can help ABC Company make better decisions related to:
- Workforce planning
- Budget allocation
- Recruitment strategies
- Salary management

---

# Future Enhancements

Possible future improvements include:
- Interactive dashboards using Plotly or Power BI
- Advanced statistical analysis
- Machine learning-based salary prediction
- Department performance analytics

---

# Author

Employee Data Analysis Project using Python and Google Colab.

---

# ML Assignment 3 — Classification

Supervised classification on the Wisconsin Diagnostic Breast Cancer dataset from scikit-learn.

Notebook: [`ML_Assignment_3_Classification.ipynb`](ML_Assignment_3_Classification.ipynb)

The notebook loads the dataset, checks for missing values, scales the features, and trains five classifiers on one stratified holdout: logistic regression, decision tree, random forest, support vector machine, and k-nearest neighbors. On the test set, logistic regression and the SVM tie for the best malignant F1 (0.9762). The decision tree is the weakest (malignant F1 0.8864). A 5-fold check on the training set ranks logistic regression first.

---

# ML Assignment 5 — Clustering

Clustering on the Iris dataset from scikit-learn. The species column is dropped before either model is fit.

Notebook: [`ML_Assignment_5_Clustering.ipynb`](ML_Assignment_5_Clustering.ipynb)

Open it in Colab and use Runtime → Run all: [Open in Colab](https://colab.research.google.com/github/abhishek12198/entriMiniProject/blob/main/ML_Assignment_5_Clustering.ipynb).

K-Means (k = 3) and Ward hierarchical clustering are fit on the four scaled measurements. One group is separated at short petals. The other two groups sit next to each other. K-Means splits that overlap more evenly (sizes 47, 50, and 53). The tree keeps a larger branch (sizes 30, 49, and 71). The adjusted Rand index between the two partitions is 0.6255.
