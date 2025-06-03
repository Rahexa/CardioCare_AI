# Heart Disease Dataset Analysis

## Overview
This repository contains a dataset and related code for analyzing heart disease data. The dataset includes various patient attributes and their corresponding heart disease diagnosis, aimed at facilitating research and predictive modeling for heart disease detection.

## Dataset Description
The dataset is provided in CSV format (`heart_disease_data.csv`) and contains the following columns:

- **age**: Age of the patient (in years)
- **sex**: Sex of the patient (1 = male, 0 = female)
- **cp**: Chest pain type (0 = typical angina, 1 = atypical angina, 2 = non-anginal pain, 3 = asymptomatic)
- **trestbps**: Resting blood pressure (in mm Hg)
- **chol**: Serum cholesterol (in mg/dl)
- **fbs**: Fasting blood sugar > 120 mg/dl (1 = true, 0 = false)
- **restecg**: Resting electrocardiographic results (0 = normal, 1 = ST-T wave abnormality, 2 = probable or definite left ventricular hypertrophy)
- **thalach**: Maximum heart rate achieved
- **exang**: Exercise-induced angina (1 = yes, 0 = no)
- **oldpeak**: ST depression induced by exercise relative to rest
- **slope**: Slope of the peak exercise ST segment (0 = upsloping, 1 = flat, 2 = downsloping)
- **ca**: Number of major vessels (0–3) colored by fluoroscopy
- **thal**: Thalassemia (0 = normal, 1 = fixed defect, 2 = reversible defect, 3 = not described)
- **target**: Diagnosis of heart disease (0 = no disease, 1 = disease)

## Installation

To use this dataset and associated code, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Rahexa/CardioCare_AI.git
   ```

2. **Install required dependencies (if any code is included):**
   ```bash
   pip install -r requirements.txt
   ```

3. Ensure you have Python 3.x and libraries like `pandas`, `numpy`, and `scikit-learn` installed for data analysis and modeling.

## Usage

### Load the Dataset
Use a tool like Python's `pandas` library to load the CSV file:

```python
import pandas as pd
data = pd.read_csv('heart_disease_data.csv')
```

### Explore the Data
Perform exploratory data analysis (EDA) to understand distributions, correlations, and patterns. Example:

```python
print(data.head())
print(data.describe())
```

### Modeling
Use the dataset for machine learning tasks such as classification to predict the target variable. Example algorithms include logistic regression, decision trees, or neural networks.

## Example Analysis

An example script (`analysis.py`) is provided to demonstrate basic data loading and visualization:

```python
import pandas as pd
import matplotlib.pyplot as plt

# Load data
data = pd.read_csv('heart_disease_data.csv')

# Basic visualization
data['age'].hist(bins=20)
plt.title('Age Distribution')
plt.xlabel('Age')
plt.ylabel('Frequency')
plt.show()
```

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature-branch
   ```
3. Make your changes and commit:
   ```bash
   git commit -m 'Add new feature'
   ```
4. Push to the branch:
   ```bash
   git push origin feature-branch
   ```
5. Create a pull request.


## Contact

For questions or feedback, please open an issue on GitHub or contact (sikderraihan693@gmail.com).
