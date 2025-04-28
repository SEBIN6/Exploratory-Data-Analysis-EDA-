# Titanic Exploratory Data Analysis (EDA)

## Overview
This project performs an **Exploratory Data Analysis (EDA)** on the Titanic dataset to uncover insights into passenger survival patterns. Using Python with Pandas, Matplotlib, and Seaborn, the analysis includes statistical summaries, visualizations, and observations about relationships between variables like passenger class, sex, age, fare, and survival status.

The dataset contains 891 passenger records with details such as survival status, class, sex, age, fare, and embarkation port. The analysis is presented in a Jupyter Notebook, with outputs exported as a PDF report.

## Objectives
- Extract insights using statistical exploration and visualizations.
- Identify relationships and trends in the Titanic dataset.
- Provide a clear summary of findings for further analysis or modeling.

## Dataset
The dataset (`train.csv`) is sourced from [Kaggle's Titanic dataset](https://www.kaggle.com/c/titanic). It includes 891 rows and 12 columns:
- **PassengerId**: Unique identifier
- **Survived**: Survival status (0 = No, 1 = Yes)
- **Pclass**: Passenger class (1 = 1st, 2 = 2nd, 3 = 3rd)
- **Name**, **Sex**, **Age**: Passenger details
- **SibSp**, **Parch**: Number of siblings/spouses and parents/children aboard
- **Ticket**, **Fare**, **Cabin**, **Embarked**: Ticket details, fare, cabin, and embarkation port (C = Cherbourg, Q = Queenstown, S = Southampton)

## Tools and Libraries
- **Python 3.x**
- **Pandas**: Data manipulation and analysis
- **Matplotlib & Seaborn**: Data visualization
- **Jupyter Notebook**: Interactive analysis environment

## Deliverables
- **Jupyter Notebook** (`titanic_eda.ipynb`): Contains the complete EDA with code, visualizations, and observations.
- **PDF Report** (`titanic_eda_report.pdf`): Summarizes findings with visuals (generated from the notebook).
- **Dataset** (`train.csv`): The Titanic dataset used for analysis.

## Analysis Tasks
1. **Statistical Exploration**:
   - Used `.describe()`, `.info()`, and `.value_counts()` to summarize numerical and categorical data.
   - Findings: 38.4% survival rate, 577 males vs. 314 females, most passengers in third class (491), missing values in Age (177) and Cabin (687).

2. **Visualizations**:
   - **Pairplot**: Relationships between Age, Fare, SibSp, Parch, colored by Survived.
   - **Correlation Heatmap**: Strong negative correlation between Pclass and Fare (-0.55), moderate positive correlation between Fare and Survived (0.26).
   - **Histograms**: Age is slightly right-skewed (mean 29.7), Fare is highly right-skewed (max 512.33).
   - **Boxplots**: Survivors are slightly younger; first-class fares are higher and more variable.
   - **Scatterplot**: Higher fares linked to better survival, regardless of age.
   - **Bar Plots**: Survival rates by Pclass (1st: 63%, 2nd: 47%, 3rd: 24%), Sex (female: 74%, male: 19%), and Embarked (Cherbourg: 55%).

3. **Key Findings**:
   - **Demographics**: Majority male, third-class passengers, with significant missing data in Age and Cabin.
   - **Survival Trends**: Higher survival for first-class, female, and younger passengers, likely due to lifeboat prioritization.
   - **Distributions**: Age and Fare distributions highlight socioeconomic disparities.
   - This EDA provides a foundation for predictive modeling.

## Observations
- **Age Distribution**: Slightly right-skewed, with a mean of 29.7, indicating many younger passengers.
- **Fare Distribution**: Highly right-skewed, with most paying low fares and a few high fares (first-class).
- **Survival by Class**: First-class passengers had the highest survival rate, reflecting better access to lifeboats.
- **Survival by Sex**: Females had a significantly higher survival rate, consistent with "women and children first."
- **Survival by Embarked**: Cherbourg passengers had the highest survival rate, possibly due to more first-class passengers.


