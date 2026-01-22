# 🌧️ Rainfall Prediction Classifier

## Project Overview
Accurately predicting rainfall is critical for agriculture, water resource management, and disaster preparedness.  
This project builds and evaluates machine learning classification models to predict whether rainfall will occur based on historical weather data.

The project compares **Logistic Regression** and **Random Forest** models, with a focus on balancing overall accuracy and **recall**, since missing a rainfall event can have significant real-world consequences.

This work was completed as the **final project** for the *Machine Learning with Python* course in the **IBM Data Science Professional Certificate**, and later refined into a portfolio-ready project.

---

## Dataset
The dataset contains daily weather observations collected over multiple years, including variables such as:
- Temperature (min/max)
- Rainfall and evaporation
- Humidity and pressure
- Wind speed and direction
- Cloud cover
- Seasonal indicators

The target variable represents whether rainfall occurred on a given day.

---

## Methodology
The project followed a standard machine learning workflow:

1. **Data Loading & Cleaning**
   - Loaded historical weather data
   - Removed rows with missing values to ensure data consistency

2. **Feature Engineering & Preprocessing**
   - Handled categorical and numerical variables using preprocessing pipelines
   - Encoded categorical features and scaled numerical features
   - Addressed potential data leakage and feature relevance
   - Ensured proper train–test splitting with stratification

3. **Model Development**
   - Implemented Logistic Regression as a baseline model
   - Built a Random Forest classifier using a preprocessing pipeline
   - Applied GridSearchCV for hyperparameter tuning

4. **Model Evaluation**
   - Evaluated models using accuracy and recall
   - Generated predictions and classification reports
   - Compared model performance to understand trade-offs

---

## Results
- The final model achieved **strong overall accuracy** on the test dataset.
- Recall was emphasized to reduce the likelihood of missing rainfall events.
- The Random Forest model demonstrated improved performance compared to the baseline Logistic Regression model.

---

## Feature Importance
Feature importance analysis highlighted that variables related to:
- **Sunshine**
- **Cloud cover**
- **Humidity**
- **Atmospheric pressure**

were among the most influential predictors of rainfall.

This aligns with real-world meteorological understanding and adds interpretability to the model.

---

## Key Insights
- Accuracy alone is not sufficient for rainfall prediction; recall is critical.
- Ensemble models such as Random Forest can better capture complex weather patterns.
- Proper preprocessing and pipeline design significantly improve model reliability.

---

## Tools & Technologies
- Python  
- Pandas, NumPy  
- Scikit-learn  
- Matplotlib, Seaborn  
- Jupyter Notebook  

---

## Future Improvements
- Experiment with additional models (e.g., Gradient Boosti
