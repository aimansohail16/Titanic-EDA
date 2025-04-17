# Titanic-EDA
This project performs a detailed Exploratory Data Analysis (EDA) on the famous Titanic dataset. The goal is to uncover meaningful patterns, clean and prepare the data, and understand the variables that may have influenced passenger survival.
## Dataset
The dataset includes details of Titanic passengers:
* Numerical Features: Age, Fare, etc.
* Categorical Features: Sex, Pclass, Embarked, etc.
* Target Variable: Survived (0 = No, 1 = Yes)
## EDA Workflow
1. ### Initial Setup
  * Loading libraries and dataset
  * Previewing structure using .head(), .info(), .describe()
2. ### Data Cleaning
  * Handling missing values:
    * Age: filled using median (due to skewed distribution)
    * Embarked & Embark_Town: filled with mode (most frequent value)
    * Cabin/Deck: dropped due to excessive missing values
  * Removed duplicate records
3. ### Univariate Analysis
  * Countplots for categorical variables
  * Histograms and boxplots for numerical variables
  * Checked distribution and outliers
4. ### Bivariate & Multivariate Analysis
  * Boxplots and countplots for survival by class, sex, etc.
  * Correlation heatmaps for numeric features
5. ### Key Insights
  * Females and upper-class passengers had higher survival rates
  * Children had better survival odds
  * Fare and age showed varied influence depending on class
