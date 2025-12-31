# Spaceship-Titanic-Analysis-and-Prediction

##  Project Overview
The goal of this project is to predict whether a passenger aboard the **Space Titanic** was
*transported to another dimension* based on demographic, socio-economic, and travel-related
attributes.

This is a **binary classification problem**, solved using statistical analysis, feature
engineering, and machine learning models. The project emphasizes **data preprocessing,
feature selection, and recall improvement**, making it suitable for real-world imbalanced
classification tasks.

---

##  Dataset Description
- **Source:** Kaggle – Space Titanic Dataset
- **Total Observations:** ~8,700 passengers
- **Target Variable:** `Transported`
  - `True` → Passenger was transported
  - `False` → Passenger was not transported

### Feature Types
- **Categorical:** HomePlanet, Destination, CryoSleep, VIP
- **Numerical:** Age, RoomService, FoodCourt, ShoppingMall, Spa, VRDeck
- **Identifier-like:** PassengerId, Cabin

  ---

##  Tools & Technologies
- **Programming Language:** Python
- **Libraries Used:**
  - NumPy
  - Pandas
  - Matplotlib / Seaborn
  - Scikit-learn

---

##  Exploratory Data Analysis (EDA)
EDA was performed to:
- Understand feature distributions
- Detect missing values
- Identify relationships between features and the target variable

Key observations:
- CryoSleep and spending-related features show strong correlation with survival
- Some numerical features are right-skewed
- Several categorical features contain missing values

---

##  Data Preprocessing
The following preprocessing steps were applied:

- **Missing Value Treatment**
  - Categorical variables: Mode imputation
  - Numerical variables: Median imputation
- **Encoding**
  - Categorical variables encoded using appropriate encoding techniques
- **Feature Scaling**
  - Numerical features scaled for model compatibility

---
##  Models Implemented
The following machine learning models were trained and evaluated:

- **Logistic Regression**
- **Support Vector Classifier**
- **K-nearest Neighbour Classifier**
- **Random Forest Classifier**
- **XGBoost Classifier**
- **Ensemble Learning using Soft Voting**

---

### Performance Summary:
| Model| Accuracy |
|--------------------|----------|
| Logistic Regression| 79.144%| 
| SVC| 80.149%|
| KNN| 77.180%|
| Random Forest| 79.845%|
| XGBoost| 80.523%|
| Soft Voting| 79.261%|
