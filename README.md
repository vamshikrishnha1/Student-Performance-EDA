# Student Performance EDA

## 📌 Project Overview

This project explores the **Student Performance in Exams** dataset to
understand how different student-related factors are associated with
exam performance.

The analysis focuses on **1,000 student records and 8 original
features**, covering student demographics, parental education, lunch
type, test preparation, and scores in math, reading, and writing.

The goal is to turn raw student data into clear insights through
**Exploratory Data Analysis (EDA)** and understand patterns in overall
exam performance.

------------------------------------------------------------------------

## 🎯 Objectives

-   Understand the structure and quality of the dataset
-   Check for missing values, duplicates, data types, and unique values
-   Explore numerical and categorical features
-   Create total and average score features
-   Analyze student performance using visualizations
-   Identify patterns related to gender, lunch, parental education, and
    race/ethnicity
-   Understand relationships between math, reading, and writing scores

------------------------------------------------------------------------

## 📊 Dataset

The dataset contains **1,000 rows and 8 columns**.

### Features

  -----------------------------------------------------------------------
  Feature                             Description
  ----------------------------------- -----------------------------------
  `gender`                            Gender of the student

  `race_ethnicity`                    Student's race/ethnicity group

  `parental_level_of_education`       Parent's highest education level

  `lunch`                             Lunch type: standard or
                                      free/reduced

  `test_preparation_course`           Whether the student completed the
                                      test preparation course

  `math_score`                        Math exam score

  `reading_score`                     Reading exam score

  `writing_score`                     Writing exam score
  -----------------------------------------------------------------------

**Dataset:** Students Performance in Exams dataset from Kaggle.

------------------------------------------------------------------------

## 🔍 Data Quality Checks

Before starting the analysis, the dataset was checked for:

-   Missing values
-   Duplicate records
-   Data types
-   Number of unique values
-   Statistical summary
-   Categories in categorical columns

### Results

-   **No missing values** were found.
-   **No duplicate records** were found.
-   Numerical statistics were reviewed to understand the score
    distributions.
-   Numerical and categorical features were separated for further
    analysis.

------------------------------------------------------------------------

## 🧮 Feature Engineering

Two additional features were created from the three subject scores:

### Total Score

``` python
df['total_score'] = (
    df['math_score'] +
    df['reading_score'] +
    df['writing_score']
)
```

### Average Score

``` python
df['average'] = df['total_score'] / 3
```

The average score was then used to study overall student performance
across different groups.

------------------------------------------------------------------------

## 📈 Exploratory Data Analysis

The project uses visualizations to explore student performance patterns.

### Analysis areas

-   Overall average score distribution
-   Performance by gender
-   Performance by lunch type
-   Performance by parental education
-   Performance by race/ethnicity
-   Relationships between numerical variables using pair plots
-   Correlations between numerical features using a heatmap

------------------------------------------------------------------------

## 💡 Key Insights

### Gender

The analysis shows that **female students tend to perform better than
male students** in terms of the average score distribution in this
dataset.

### Lunch

Students with **standard lunch show higher performance distributions**
compared with students with free/reduced lunch.

The analysis also shows this pattern for both male and female students.

### Parental Education

The overall analysis does not show a strong general relationship between
parental education and student performance.

However, some differences appear when the data is further split by
gender.

### Race/Ethnicity

Students in **Group A and Group B tend to have lower performance
distributions** compared with other groups in this dataset.

------------------------------------------------------------------------

## 🛠️ Tools & Technologies

-   **Python**
-   **Pandas** -- Data manipulation and analysis
-   **NumPy** -- Numerical operations
-   **Matplotlib** -- Data visualization
-   **Seaborn** -- Statistical visualization
-   **Jupyter Notebook** -- Analysis environment

------------------------------------------------------------------------

## 📁 Project Structure

``` text
Student-Performance-EDA/
│
├── 2.0-Student Performance EDA.ipynb
├── stud.csv
└── README.md
```

------------------------------------------------------------------------

## ▶️ How to Run the Project

### 1. Clone the repository

``` bash
git clone <your-repository-url>
cd Student-Performance-EDA
```

### 2. Install the required libraries

``` bash
pip install pandas numpy matplotlib seaborn jupyter
```

### 3. Start Jupyter Notebook

``` bash
jupyter notebook
```

### 4. Open the notebook

Open:

``` text
2.0-Student Performance EDA.ipynb
```

Make sure the dataset file is available in the expected location before
running the notebook.

------------------------------------------------------------------------

## 📌 What This Project Demonstrates

This project demonstrates my ability to:

-   Work with a real-world dataset
-   Perform data quality checks
-   Clean and prepare data for analysis
-   Create meaningful features
-   Analyze numerical and categorical data
-   Build clear visualizations
-   Extract useful patterns from data
-   Communicate analytical findings in a simple way

------------------------------------------------------------------------

## 👤 Author

**Vamshi Krishna Bodige**

