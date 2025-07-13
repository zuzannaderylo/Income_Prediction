# Income Prediction using Census Data
This project explores the Adult Income dataset from the UCI Machine Learning Repository to analyze and predict whether individuals earn more or less than $50,000 per year. The dataset contains demographic and employment-related features, making it ideal for applying data preprocessing, exploratory data analysis (EDA), unsupervised learning, and supervised classification models.

## Project Overview
- **Dataset**: [UCI Adult Income Dataset](https://archive.ics.uci.edu/ml/datasets/adult)
- **Goal**: Identify key demographic and employment-related features that influence income level and can be used to predict it. 
- **Techniques used**:
  - Exploratory Data Analysis (EDA)
  - Data Cleaning and Preprocessing
  - Dimensionality Reduction (PCA)
  - Clustering (KMeans, T-SNE visualization)
  - Classification (Support Vector Machine, Logistic Regression)
 
📌 **This project was a team effort, but further description focuses on my individual contribution** to the project: Exploratory Data Analysis (EDA) and Data Preprocessing. Although I was helping with other parts, I was not the main contributor. 

## 🔍 My Contributions
### 1. Exploratory Data Analysis (EDA)
- Summary statistics for numerical and categorical features
- Visual analysis using histograms, bar plots, and correlation heatmaps
- Outlier detection using Z-score and IQR methods
- Analysis of class imbalance in target variable (`income`)

### 2. Data Preprocessing
- Converted missing values (`?`) into `NaN` and compared:
  - Row removal
  - Mode imputation
  - KNN imputation (chosen method)
- Grouped and simplified categorical variables (e.g., marital status)
- Encoded categorical features (label encoding & one-hot encoding)
- Standardized numerical features using `StandardScaler`
- Evaluated class balancing using SMOTE (decided against it to preserve precision)

### 3. Documentation
- Wrote detailed summary and rationale for each preprocessing step
- Analyzed trade-offs (e.g., imputation bias vs. data loss)
 
## Used tools
- Python
- Pandas, NumPy
- Scikit-learn
- Seaborn, Matplotlib
- Jupyter Notebook

---

*This project was part of a Data Mining course at IT University of Copenhagen (2025).*
