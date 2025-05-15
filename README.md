# 🏡 Airbnb Price Prediction Model

This project focuses on building a machine learning model to predict Airbnb listing prices using data cleaning, feature engineering, exploratory data analysis (EDA), and model evaluation. The final model achieves **99% accuracy on unseen data**.

---

## 📌 Project Workflow

### 1. Load and Observe Dataset
- The Airbnb dataset was loaded and examined for structure, data types, missing values, and basic statistics.

---

### 2. Clean Dataset 🧼
- **Feature Descriptions and Relevance**: Each feature was defined and assessed for relevance to price prediction.
- **Dropped Columns**: Redundant or irrelevant features such as identifiers (`id`, `host id`), and poorly populated fields were removed.
  
---

### 3. Feature Engineeringm 🛠
- **Categorical Features**: Encoded using techniques like one-hot encoding.
- **Continuous Features**: Handled outliers and prepared for standardization.
- **Datetime Features**: Extracted useful components (like year or month) from dates such as `last review`.
- **Missing Values**: Addressed using strategies like imputation (mean/mode) or KNN imputer where appropriate.

---

### 4. Standardize Continuous Features ⚖
- Applied `StandardScaler` to normalize continuous variables so they contribute equally to model training.

---

### 5. Exploratory Data Analysis (EDA) 🔎
- Visualized relationships between price and other variables using plots such as:
  - Price vs. Room Type
  - Price vs. Neighbourhood
  - Price vs. Availability
  - Correlation matrix of numerical features

---

### 6. Build Model 🏗
- **Split Data**: Divided into training and test sets.
- **Train Model**: Fitted using regression algorithms with hyperparameter tuning for best performance.

---

### 7. Evaluate Model Performance 🤓
- Evaluated using **Root Mean Square Error (RMSE)** on test data.
- Visualized residuals and compared predicted vs. actual values.
- Final model was tested on **unseen data** and compared for real-world performance.

---

## ✅ Final Result 
- The model achieved **99% accuracy on unseen data**, demonstrating strong generalization capability.

---

## 📁 Files Included
- `notebook.ipynb`: Contains the full code and analysis
- `model.pkl`: Trained model file 
- `airbnb_data.csv`: Input dataset
- `README.md`: Project documentation

---

## 📌 Requirements
- Python 3.x
- pandas
- numpy
- scikit-learn
- matplotlib / seaborn
- jupyter notebook 

---

## 📣 Acknowledgments
Thanks to Airbnb for the data and sci-kit klearn for the open-source ML tools that made this project possible. Pandas I'm greatful too, wouldn't be able to do this without you 😏

---

## 🚀 Future Improvements
- Deploy the model via a web API
- Use AutoML frameworks like `TPOT` or `H2O`

---
