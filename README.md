# Cardiovascular Disease Prediction ❤️📊

A machine learning classification project that analyzes patient medical records to predict the 10-year risk of future coronary heart disease (CHD).

## 🚀 Project Overview

Cardiovascular diseases are the leading cause of death globally. Early detection of high-risk patients can drastically improve preventative care and treatment outcomes. This project builds a predictive model that evaluates a combination of demographic, behavioral, and medical risk factors to determine whether a patient is at risk of developing heart disease within the next ten years.

## ⚙️ Methodology

1. **Data Preprocessing**: 
   - Loaded the Framingham Heart Study dataset.
   - Handled missing values by dropping incomplete records (`dropna()`) to ensure the integrity of the training process.
2. **Feature Engineering**:
   - Separated the dataset into feature vectors (`X`) containing risk factors (e.g., age, blood pressure, cholesterol, smoking habits) and the target label (`y`), which represents `TenYearCHD`.
3. **Model Selection & Training**:
   - Split the data into an 70% training and 30% testing set using `train_test_split`.
   - Initialized and trained a **Decision Tree Classifier** to map the non-linear relationships between the medical features and the disease outcome.
4. **Evaluation**:
   - Evaluated the model against the unseen test data to calculate the overall predictive accuracy.

## 📊 Dataset

The model is trained on the renowned **Framingham Heart Study** dataset (`framingham.csv`). It includes over 4,000 records of patients from Framingham, Massachusetts, tracking 15 attributes including:
- **Demographic**: Sex, Age
- **Behavioral**: Current Smoker, Cigs Per Day
- **Medical History**: BP Meds, Prevalent Stroke, Prevalent Hyp, Diabetes
- **Current Medical**: Total Cholesterol, Sys BP, Dia BP, BMI, Heart Rate, Glucose

## 🛠️ Tech Stack & Libraries Used

- **Data Manipulation:** Pandas
- **Machine Learning Algorithm:** Scikit-learn (`DecisionTreeClassifier`)
- **Evaluation Metrics:** Scikit-learn (`accuracy_score`, `train_test_split`)

## 📈 Key Outcomes

- Successfully built an end-to-end classification pipeline for medical tabular data.
- Demonstrated the use of Decision Trees for interpretable clinical predictions, allowing healthcare providers to understand the splits (e.g., if Age > 50 and Smoker = Yes) that lead to high-risk predictions.

---
*This repository is part of my AI Engineer / Data Scientist Portfolio.*
