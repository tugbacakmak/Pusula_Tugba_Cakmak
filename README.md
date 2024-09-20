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

## Key Steps in the Analysis
### Data Loading and Cleaning:

Handled missing values in numerical columns using mean imputation.
Categorical columns were filled with placeholders like 'Bilinmeyen' for unknown values.

### Feature Engineering:
Derived age from the birth date.
Calculated drug usage duration in days.

### Exploratory Data Analysis (EDA):
Visualized distributions of weight, height, and side effects.
Analyzed relationships between gender, chronic diseases, and side effects.
Examined geographic distribution of reported side effects.

### Data Preparation:

Encoded categorical variables (e.g., blood type, gender).
Standardized numerical features like weight, height, and drug duration.
Split the dataset into training and test sets for further modeling.

### Results and Insights

#### Common Side Effects: Kabızlık (constipation), Yorgunluk (fatigue), and Çarpıntı (palpitations) were frequently reported.
#### Drug-Specific Findings: Some drugs, like trifluoperazine and fluphenazine, were linked to a higher number of side effects.
#### Chronic Diseases: Patients with conditions such as hypertension or COPD generally had higher average weights.

### Final Notes

The project is designed to provide insights into the relationships between drug usage and side effects, with a focus on making the data ready for predictive modeling in future steps.
