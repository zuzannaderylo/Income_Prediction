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
 
📌 **This project was a team effort, but further description focuses on my individual contribution** to the project: Exploratory Data Analysis (EDA) and Data Preprocessing. 

## My Contributions
### 1. Exploratory Data Analysis (EDA)
- Summary statistics for numerical and categorical features
- Visual analysis using histograms, bar plots, and correlation heatmaps
- Outlier detection using Z-score and IQR methods
- Analysis of class imbalance in target variable (`income`)

### 2. Missing Values Analysis
- Found ~7.4% of the data had missing values in `workclass`, `occupation`, and `native-country`
- Implemented and **compared three strategies**:
  - Row deletion (simple but data-destructive)
  - Mode imputation (biased some categorical distributions)
  - **KNN imputation** – selected for preserving feature distribution and improving model performance (F1, AUC)

### 3. Data Preprocessing
- Converted missing values (`?`) into `NaN` and used KNN imputation for filling missing values
- Grouped and simplified categorical variables (e.g., marital status)
- Discretized age into bins
- Encoded categorical features
  - One-hot encoding for unsupervised tasks
  - Label/manual encoding for supervised learning
- Standardized numerical features using `StandardScaler`
 
## Used tools
- Python
- Pandas, NumPy
- Scikit-learn
- Seaborn, Matplotlib
- Jupyter Notebook

## Author
**Zuzanna Emilia Derylo**  
📧 zuzia.derylo@gmail.com
🔗 [GitHub Profile](https://github.com/zuzannaderylo)

---

*This project was part of a Data Mining course at IT University of Copenhagen (2025).*
