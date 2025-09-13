# analysis-on-predicting-diabetes-using-ML


## Diabetes Risk Prediction with Machine Learning

## Project Summary
Diabetes is a chronic lifestyle-related illness caused by the body’s inability to use insulin properly. It results in high blood sugar and can lead to complications affecting the heart, kidneys, and vision.  
Predicting the risk early is essential for timely intervention and preventive healthcare.  

This project applies *machine learning techniques* to predict whether a person is likely to have diabetes, using health indicators such as *glucose level, BMI, age, and family history*.

---

##  Goals
- Explore health data and identify the most influential features for diabetes detection.  
- Build and train *machine learning models* to classify individuals as diabetic or non-diabetic.  
- Evaluate and compare multiple algorithms to determine the most effective approach.  

---

##  Dataset Information
- *Total Features:* 8 independent variables + 1 target (Outcome)  
- *Data Challenges:*  
  - Zero values in some fields (treated as missing data)  
  - Presence of outliers  
  - Slight imbalance between diabetic and non-diabetic cases  
- *Preprocessing Applied:*  
  - Handling missing/invalid values  
  - Outlier detection and correction  
  - Feature scaling and normalization  
  - Multicollinearity checks  

---

##  Data Exploration
- Class distribution: *71.5% non-diabetic vs 28.5% diabetic*  
- Visuals: Pie charts, histograms, count plots, pair plots, and heatmaps  
- Findings: *Glucose, **BMI, and **Age* emerged as the strongest predictors  

---

##  Machine Learning Models
| Algorithm            | Accuracy (70–30 Split) |
|----------------------|-------------------------|
| Logistic Regression  | 0.8072 |
| Decision Tree        | 0.724  |
| KNN                  | 0.830  |
| SVM                  | 0.830  |
| Bagging              | 0.802  |
| AdaBoost             | 0.802  |
| Random Forest        | 0.802  |
| Gradient Boost       | 0.7709 |
| XGBoost              | 0.7709 |
| ANN                  | Implemented |

- *Top Performers:* *SVM and KNN* (~83% accuracy)  
- *Ensemble models* (Bagging, AdaBoost, Random Forest) provided stable results.  

---

##  Insights
- *Glucose* levels were the most influential factor.  
- *BMI and Age* also contributed strongly to predictions.  
- *Decision Tree* performed the weakest (~72%).  
- Ensemble methods offered better balance and generalization compared to standalone models.  

---

##  Final Takeaways
- Data required careful preprocessing before model training.  
- Class imbalance slightly favored non-diabetic predictions.  
- Ensemble techniques, especially *Boosting*, are the most practical choice for real-world deployment.  

---

##  Running the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/diabetes-ml-prediction.git
   cd diabetes-ml-prediction
