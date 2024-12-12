# Heart Disease Prediction using Machine Learning

### Overview

This project involves the use of the Heart Disease Dataset to build a machine learning model that predicts whether a patient has heart disease based on various health-related features. The dataset provides a wealth of information, including patient demographics, health measurements, and test results, making it a great opportunity for data exploration and predictive modeling.

### Dataset

The dataset consists of 606 rows and 14 columns. These columns represent different health attributes, such as:

- age: Age of the patient
- sex: Gender of the patient (0 = female, 1 = male)
- cp: Chest pain type (0 = typical angina, 1 = atypical angina, 2 = non-anginal pain, 3 = asymptomatic)
- trestbps: Resting blood pressure (in mm Hg)
- chol: Serum cholesterol (in mg/dl)
- fbs: Fasting blood sugar > 120 mg/dl (1 = true, 0 = false)
- restecg: Resting electrocardiographic results (0 = normal, 1 = stt abnormality, 2 = lv hypertrophy)
- thalach: Maximum heart rate achieved
- exang: Exercise-induced angina (1 = yes, 0 = no)
- oldpeak: ST depression induced by exercise relative to rest
- slope: The slope of the peak exercise ST segment
- ca: Number of major vessels colored by fluoroscopy (0 to 3)
- thal: Thalassemia (0 = normal, 1 = fixed defect, 2 = reversible defect)
- target: Heart disease presence (1 = disease present, 0 = disease absent)

### Data Preprocessing

The dataset was cleaned and preprocessed to prepare for training. The steps included:

- Handling missing values (if any)
- Encoding categorical variables like sex, cp, restecg, and thal into numerical values using one-hot encoding or label encoding
- Feature scaling using StandardScaler to ensure that all features are on the same scale

### Model Building

A Logistic Regression model was used to predict the presence of heart disease based on the health attributes provided in the dataset. The model was trained on a training set and evaluated on a test set using Accuracy: 81.97%.

### Key Findings

- The **accuracy** of the model is approximately **82%**, indicating that it is performing reasonably well.
- The model performs better in predicting cases where heart disease is present (`target = 1`), with **higher recall (89%)** for detecting heart disease patients.
- The **precision and recall** for predicting no heart disease (`target = 0`) are lower, but still reasonable, with **precision of 82%** and **recall of 72%**.

### Next Steps

- **Model Improvement**: Experiment with more advanced models like **Random Forest**, **Gradient Boosting**, or **XGBoost** to potentially improve performance.
- **Handling Class Imbalance**: Consider using techniques like **SMOTE** (Synthetic Minority Over-sampling Technique) or **class weight adjustment** to handle class imbalance in the dataset.
- **Feature Engineering**: Explore new features or combine existing ones to enhance model accuracy.

### Source

https://www.kaggle.com/datasets/thisishusseinali/uci-heart-disease-data
