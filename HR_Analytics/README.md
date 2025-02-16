
### **Employee Attrition Prediction**  

- **Objective**: Predict employee attrition using machine learning models.  
- **Dataset**: Contains employee details such as department, years at company, overtime, and attrition status.  
- **Exploratory Data Analysis (EDA)**:  
  - Visualized attrition trends based on years at the company, department, and overtime status.  
  - Identified key factors contributing to attrition.  
- **Models Used**:  
  - **Ridge Classifier**: High accuracy in predicting non-attrition cases but struggled with false negatives.  
  - **XGBoost Classifier**: Improved recall and detected attrition cases better.  
- **Performance Metrics**:  
  - Compared confusion matrices for both models.  
  - Ridge: Lower false positives, higher false negatives.  
  - XGBoost: Better recall with a trade-off in false positives.  
- **Tools & Libraries**: Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost.  
- **Outcome**: XGBoost achieved better balance in predicting attrition cases.  


