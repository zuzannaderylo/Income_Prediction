# Income Prediction using Census Data
This project explores the Adult Income dataset from the UCI Machine Learning Repository to analyze and predict whether individuals earn more or less than $50,000 per year. The dataset contains demographic and employment-related features, making it ideal for applying data preprocessing, exploratory data analysis (EDA), unsupervised learning, and supervised classification models.

## Repository Structure

| File | Description |
|------|-------------|
| `Assignment.ipynb` | Main analysis notebook with EDA, preprocessing, and transformation |
| `MissingValuesAnalysis.ipynb` | Comparison of missing data strategies (KNN, Mode, Deletion) |
| `adult.csv` | Cleaned dataset (from UCI Adult Income dataset) |
| `requirements.txt` | Required Python libraries |
| `README.md` | This file |

## Project Overview
- **Dataset**: [UCI Adult Income Dataset](https://archive.ics.uci.edu/ml/datasets/adult)
- **Goal**: Identify key demographic and employment-related features that influence income level and can be used to predict it. 
- **Techniques used**:
  - Exploratory Data Analysis (EDA)
  - Data Cleaning and Preprocessing
  - Unsupervised learning: Dimensionality Reduction (PCA), Clustering (KMeans, T-SNE visualization)
  - Supervised learning: Support Vector Classification, Logistic Regression
 
📌 **This project was a team effort. The following description focuses on my individual contribution to the project: Exploratory Data Analysis (EDA), and Data Cleaning and Preprocessing.**

## My Contributions
### 1. Exploratory Data Analysis (EDA)
- Summary statistics for numerical and categorical features
- Visual analysis using histograms, bar plots, and correlation heatmaps
- Outlier detection using Z-score and IQR methods
- Analysis of class imbalance in target variable (`income`)
- Identified skewness in capital-gain and capital-loss, with most values concentrated at 0
- Noted class imbalance in the target variable: ~76% earn <=$50K

### 2. Missing Values Strategy Analysis
- Identified ~7.4% missing data in `workclass`, `occupation`, and `native-country`
- Implemented and evaluated three imputation methods:
  - **Row Deletion** – simple but removed valuable data
  - **Mode Imputation** – distorted categorical distributions
  - **KNN Imputation** – chosen for best balance between accuracy and distribution preservation (improved F1 and AUC)

### 3. Data Cleaning and Preprocessing
- Converted missing values (`?`) into `NaN` and used KNN imputation for filling missing values
- Grouped and simplified categorical variables (e.g., marital status)
- Discretized age into bins
- Encoded categorical features
  - One-hot encoding for unsupervised tasks
  - Label/manual encoding for supervised learning
- Standardized numerical features using `StandardScaler`

## Results Summary
- Best model: Support Vector Classifier (F1 > $50K: 0.67)
- Top predictive features: capital-gain, marital-status, education
- KNN imputation outperformed other strategies and preserved data distribution

## Installation 
To run the project locally, follow these steps:

### 1. Clone the repository
```bash
git clone https://github.com/zuzannaderylo/income-prediction.git
cd income-prediction
```

### 2. Create a virtual environment (optional)
```
python -m venv venv
source venv/bin/activate
```

### 3. Install dependencies
```
pip install -r requirements.txt
```

### 4. Launch Jupyter Notebook
```
jupyter notebook
```
Open Assignment.ipynb to run the full pipeline, including EDA, data cleaning, modeling, and evaluation.

Open MissingValuesAnalysis.ipynb to compare different imputation strategies.

## Used tools
- Python
- Pandas, NumPy
- Scikit-learn
- Seaborn, Matplotlib
- Jupyter Notebook


## Author
**Zuzanna Emilia Derylo**  
📧 zuzia.derylo@gmail.com
🔗 [LinkedIn Profile](https://www.linkedin.com/in/zuzannaderylo/)
🔗 [GitHub Profile](https://github.com/zuzannaderylo)

---

*This project was part of a Data Mining course at IT University of Copenhagen (2025).*
