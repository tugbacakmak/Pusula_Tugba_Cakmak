# Drug Side Effects Data Analysis

## Overview
This project is focused on analyzing a dataset related to drug side effects. The main objective is to perform exploratory data analysis (EDA) and preprocess the dataset for predictive modeling. The dataset contains information such as drug names, side effects, patient demographics, and more. The analysis includes handling missing values, encoding categorical variables, normalizing numerical features, and visualizing relationships within the data.

The final step prepares the data for predictive modeling, ensuring that it is clean and standardized.


## Getting Started
### Prerequisites
To run the code, ensure you have the following libraries installed:
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`

You can install them using pip:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

Code Explanation
1. Data Loading and Inspection
The dataset is loaded using Pandas from an Excel file (side_effect_data 1.xlsx). The initial inspection of the data was performed to understand its structure, including the types of columns and any missing values. This step includes checking the first and last few rows, and determining how many null values are present.

2. Handling Missing Values
To ensure the dataset is ready for further analysis, missing values were handled using various techniques:

Numerical Columns (e.g., Kilo, Boy): Missing values were imputed using the mean strategy via SimpleImputer from Scikit-learn.
Categorical Columns (e.g., Cinsiyet, Kronik Hastaliklarim): Missing categorical values were filled with the placeholder 'Bilinmeyen', indicating unknown data.
3. Feature Engineering
Age Calculation: The age of each patient was derived from the Dogum_Tarihi (birth date) column.
Drug Usage Duration: The duration for which each drug was used was calculated by subtracting the Ilac_Baslangic_Tarihi from the Ilac_Bitis_Tarihi to get the number of days.
4. Exploratory Data Analysis (EDA)
Several visualizations were created to better understand the relationships in the data:

Distributions of key variables such as Kilo (weight), Boy (height), and Cinsiyet (gender).
Side Effect Analysis: Visualizations were created to show the frequency of different side effects and how they vary by factors like gender, age, and geographic location.
Drug-Specific Analysis: The most common drugs and their associated side effects were highlighted using bar charts.
Chronic Diseases: The relationship between chronic diseases and patients' average weight was explored and visualized.
Correlation Analysis: A heatmap was created to show the correlations between numerical features like weight, height, and age.
5. Data Preprocessing for Modeling
The dataset was prepared for predictive modeling:

Encoding Categorical Variables: Categorical variables such as Kan Grubu (blood type) were one-hot encoded, while Cinsiyet (gender) was label-encoded to be used in models.
Normalization: The numerical features such as weight, height, age, and drug duration were standardized using StandardScaler to ensure all values are on the same scale.
Train-Test Split: The data was split into training and testing sets for future model development.
6. Key Findings
The most common side effects include symptoms like Kabızlık (constipation), Yorgunluk (fatigue), and Çarpıntı (palpitations).
Gender differences in the occurrence of side effects were observed.
Some drugs, such as trifluoperazine and fluphenazine, were associated with the highest number of side effect reports.
Patients with chronic diseases such as Hipertansiyon (hypertension) or KOAH (COPD) tended to have higher average weights.
Geographical Insights: Patients from different cities reported varying types and frequencies of side effects.
