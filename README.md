Titanic Dataset – Exploratory Data Analysis (EDA)
Objective
The goal of this project is to perform Exploratory Data Analysis (EDA) on the Titanic dataset to uncover trends, patterns, and relationships between passenger attributes and survival outcomes.
This task builds skills in:

Data cleaning

Handling missing values & outliers

Data visualization

Statistical & trend analysis

Dataset
The dataset contains details about passengers aboard the Titanic, including:

Numerical columns: Age, Fare, SibSp, Parch, PassengerId, Pclass, Survived

Categorical columns: Sex, Cabin, Embarked, Name, Ticket

Source: Titanic dataset (Kaggle / Seaborn)

Tools & Libraries
Python: Pandas, NumPy, Seaborn, Matplotlib

Environment: Jupyter Notebook

Visualization Functions:

sns.pairplot()

sns.heatmap()

Histograms

Boxplots

Scatterplots

Countplots

EDA Workflow
Data Overview

Used .info(), .describe(), .isnull().sum() to understand structure and missing values.

Missing Value Handling

Age: Imputed with median grouped by Pclass & Sex.

Cabin: Created Cabin_Available flag and dropped original column.

Embarked: Filled missing with most common value ('S').

Outlier Detection & Capping

Detected using IQR method.

Capped extreme values for Age, SibSp, Parch, and Fare.

Visual Analysis

Pairplot: Showed survival trends by age, fare, and class.

Heatmap: Highlighted correlations between Fare, Pclass, and survival.

Histograms: Showed distribution of numeric features.

Boxplots: Verified outlier treatment.

Scatterplots: Visualized Age vs Fare by survival.

Countplots: Displayed survival by gender and passenger class.

Observations

Females had a higher survival rate than males.

1st class passengers survived at higher rates than 2nd and 3rd.

Higher fare generally linked to higher survival probability.

Most passengers traveled alone.

Overall Findings

Survival probability is influenced by gender, class, and fare.

Economic status and small family groups increased survival chances.

Age alone was not a strong survival predictor but children had slightly better outcomes.

Deliverables
Jupyter Notebook (titanic_eda.ipynb) – Contains full code, visualizations, and step-by-step analysis.

PDF Report – Exported summary 

README.md – Project description and workflow (this file)
