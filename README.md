#  Skin Disorder Detection using Machine Learning

This project focuses on detecting and classifying six common types of **Erythemato-Squamous Diseases (ESD)** using supervised machine learning algorithms. These diseases are clinically challenging to distinguish, and this project aims to assist dermatologists in improving diagnostic accuracy using structured patient data.

---

##  Project Summary

- **Objective:** Predict the correct ESD type (e.g., psoriasis, seborrheic dermatitis) based on clinical and histopathological features.
- **Dataset:** Contains 366 patient records with 35 attributes:
  - 12 features clinically evaluated
  - 23 features derived from skin sample histopathology

---

##  Data Preprocessing

- Replaced invalid and zero values in the `Age` attribute with the column mean.
- Dropped 13 highly correlated attributes to avoid **overfitting**, including:
  - `itching`, `koebner_phenomenon`, `melanin_incontinence`, `eosinophils_in_the_infiltrate`, and others.
- Applied **correlation matrix analysis** to optimize feature selection and reduce noise.

---

##  Models Implemented

| Model                   | Accuracy |
|------------------------|----------|
| Decision Tree          | 93%      |
| Random Forest          | 93%      |
| Support Vector Machine | 92%      |
| XGBoost                | 93%      |
| Logistic Regression    | 92%      |

>  **Random Forest** was selected for final prediction due to its consistency and robustness in multiclass classification.

---

##  Technologies Used

- **Language:** Python 3.x
- **Libraries:**  
  - `pandas`, `numpy` for data manipulation  
  - `matplotlib`, `seaborn` for visualization  
  - `scikit-learn` for model building  
  - `xgboost` for gradient boosting

---

##  How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/vaishnavak2001/skin-disorder-detection.git
   cd skin-disorder-detection
