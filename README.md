# DATA-PIPELINE-DEVELOPMENT

Company: CODTECH IT SOLUTIONS
Name: Jonna Nikhil
Intern Id: CT04DF1123
Domain: Data Science
Duration: 4 Weeks
Mentor: Neela Santhosh

# Task 1 – Data Pipeline Development

## Overview

This project focuses on building an automated ETL (Extract, Transform, Load) pipeline using Python for the **Extrovert vs. Introvert Personality Traits Dataset**. The objective is to clean, transform, and analyze behavioral data for personality classification.

This project is submitted as **Task 1 – Data Pipeline Development** for the **Data Science Internship at CODTECH IT SOLUTIONS PVT. LTD.**

Dive into the Extrovert vs. Introvert Personality Traits Dataset, a rich collection of behavioral and social data designed to explore the spectrum of human personality. This dataset captures key indicators of extroversion and introversion, making it a valuable resource for psychologists, data scientists, and researchers studying social behavior, personality prediction, or data preprocessing techniques.

Context

Personality traits like extroversion and introversion shape how individuals interact with their social environments. This dataset provides insights into behaviors such as time spent alone, social event attendance, and social media engagement, enabling applications in psychology, sociology, marketing, and machine learning. Whether you're predicting personality types or analyzing social patterns, this dataset is your gateway to uncovering fascinating insights.

---

## Dataset Description

**Title**: Extrovert vs. Introvert Behavior Data  
**Source**: [Kaggle Dataset](https://www.kaggle.com/datasets/rakeshkapilavai/extrovert-vs-introvert-behavior-data)  
**File Used**: `personality_dataset.csv`  
**Size**: 2,900 rows × 8 columns  
**Target Variable**: `Personality` (Extrovert/Introvert)

### Features:

| Feature                   | Description                                               |
|--------------------------|-----------------------------------------------------------|
| `Time_spent_Alone`       | Hours spent alone daily (0–11)                            |
| `Stage_fear`             | Presence of stage fright (`Yes` / `No`)                   |
| `Social_event_attendance`| Frequency of attending social events (0–10)               |
| `Going_outside`          | Frequency of going outside (0–7)                          |
| `Drained_after_socializing` | Feeling drained after socializing (`Yes` / `No`)       |
| `Friends_circle_size`    | Number of close friends (0–15)                            |
| `Post_frequency`         | Social media post frequency (0–10)                        |
| `Personality`            | Target variable: Extrovert / Introvert                    |

Data Quality: Includes some missing values, ideal for practicing imputation and preprocessing.
Format: Single CSV file, compatible with Python, R, and other tools.*

Data Quality Notes

Contains missing values in columns like Time_spent_Alone and Going_outside, offering opportunities for data cleaning practice.
Balanced classes ensure robust model training.
Binary categorical variables simplify encoding tasks.
Potential Use Cases

Build machine learning models to predict personality types.
Analyze correlations between social behaviors and personality traits.
Explore social media engagement patterns.
Practice data preprocessing techniques like imputation and encoding.
Create visualizations to uncover behavioral trends.

---

## ETL Pipeline Process

### 1. **Extraction**
- Loaded raw data using `pandas`.

### 2. **Transformation**
- Removed duplicates.
- Handled missing values using `SimpleImputer`.
- Encoded categorical columns using `LabelEncoder`.
- Scaled numerical features using `StandardScaler`.

### 3. **Loading**
- Saved the cleaned data to `personality_dataset_cleaned.csv`

---

## Visualizations

All visualizations are saved in the 'DATA-PIPELINE-DEVELOPMENT' folder.

| Visualization                     | Description                                |
|----------------------------------|--------------------------------------------|
| Missing Values Heatmap           | Visual check for nulls                     |
| Personality Distribution         | Count of Extroverts vs. Introverts         |
| Correlation Heatmap              | Relationships among features               |
| Pairplot                         | Pairwise feature analysis (sample subset)  |
| Boxplots                         | Outlier detection for numerical features   |
| Distribution Plots               | KDE + histogram for each numeric column    |

---

## Output Files

- `personality_dataset.csv` – Raw dataset
- `personality_etl_pipeline.ipynb` – ETL pipeline notebook
- `personality_dataset_cleaned.csv` – Cleaned dataset
- 'DATA-PIPELINE-DEVELOPMENT' – Contains all visualizations in `.png` format

---

## How to Run

1. Clone this repo:
```bash
git clone https://github.com/Nikhiljonna/Data-Pipeline-Development.git
