# 📊 Customer Churn Prediction – Neo Telecom  

## 🚀 Project Overview  

Customer retention is a **critical challenge** for telecom companies. As a Data Scientist at **Neo Telecom**, this project aims to analyze customer behavior, extract insights, and build **predictive models** to reduce churn rates. The study involves **data manipulation, visualization, and machine learning techniques** to identify high-risk customers and improve retention strategies.  

---

## 🎯 Project Objective  

✔ Identify key factors leading to customer churn.  
✔ Analyze customer demographics, payment methods, contract types, and tenure.  
✔ Build **predictive models** to classify churned and non-churned customers.  
✔ Provide data-driven recommendations to **reduce churn rates** and increase revenue.  

---

## 📂 Dataset Information  

The dataset contains **7,043 customer records** with **21 features**, including demographics, contract details, payment methods, and churn status.  

**Key Features:**  
- **CustomerID** – Unique identifier for customers.  
- **Gender** – Male or Female.  
- **SeniorCitizen** – 1 (Yes), 0 (No).  
- **Tenure** – Number of months the customer has stayed with the company.  
- **InternetService** – DSL, Fiber Optic, or No.  
- **Contract** – Month-to-month, One-year, Two-year.  
- **PaymentMethod** – Electronic check, Mailed check, Bank transfer, Credit card.  
- **MonthlyCharges** – Customer’s monthly bill.  
- **TotalCharges** – Total amount charged.  
- **Churn** – Whether the customer has churned (Yes/No).  

---

## 📌 Key Insights & Findings  

🔹 **Churn Rate:** **26.5%** of customers have left the company.  
🔹 **High-Risk Customers:**  
   - Customers with **monthly charges > $100** or **tenure < 6 months** are more likely to churn.  
   - **Senior male citizens using electronic checks** have a **45% churn rate** (highest among groups).  
   - Customers with **month-to-month contracts** have a **60% churn rate**, while **two-year contracts** have only **3% churn**.  
🔹 **Internet Service Impact:**  
   - **Fiber optic users** churn more (**42% churn rate**) compared to **DSL users (24%)** and **No internet (10%)**.  
🔹 **Payment Method Impact:**  
   - **Electronic check users** have a **48% churn rate**, the highest among payment types.  

---

## 🔧 Tech Stack  

- **Programming:** Python 🐍  
- **Data Processing:** Pandas, NumPy  
- **Data Visualization:** Matplotlib, Seaborn  
- **Machine Learning:** Scikit-learn  
- **Model Deployment (Future Work):** Flask, Streamlit  
- **Environment:** Jupyter Notebook, Anaconda  

---

## 🚀 Tasks Performed  

### 🛠 1️⃣ Data Manipulation  
✔ Extracted **specific columns** for targeted analysis.  
✔ Filtered customers based on **demographics, contract types, and payment methods**.  
✔ Selected a **random sample of 333 records** for further study.  
✔ Counted unique values in the **Churn** column.  

---

### 📊 2️⃣ Data Visualization  
✅ **Bar Plot** – Internet Service distribution.  
✅ **Histogram** – Customer tenure distribution.  
✅ **Scatter Plot** – **Monthly Charges vs. Tenure** (trend analysis).  
✅ **Box Plot** – Tenure distribution across contract types.  

---

### 🤖 3️⃣ Machine Learning Models  

#### **🔵 Linear Regression (Predicting Monthly Charges)**  
📌 **Objective:** Predict **MonthlyCharges** based on **Tenure**.  
✔ Split dataset: **70% train, 30% test**.  
✔ **RMSE:** **$29.3** (prediction error).  

---

#### **🟢 Logistic Regression (Churn Prediction)**  
📌 **Objective:** Predict **Churn** based on **Monthly Charges & Tenure**.  
✔ Split dataset: **65% train, 35% test**.  
✔ **Accuracy (Single Feature - Monthly Charges):** **73%**.  
✔ **Accuracy (Multiple Features - Tenure & Monthly Charges):** **78%**.  

---

#### **🌲 Decision Tree (Churn Classification)**  
📌 **Objective:** Classify customers as **Churn (Yes/No)** based on **Tenure**.  
✔ Split dataset: **80% train, 20% test**.  
✔ **Accuracy:** **81%**.  

---

#### **🌳 Random Forest (Churn Classification - Best Model)**  
📌 **Objective:** Improve churn prediction with multiple decision trees.  
✔ Split dataset: **70% train, 30% test**.  
✔ **Accuracy:** **86%**.  
✔ **Feature Importance:**  
   - **Tenure** (52%)  
   - **Monthly Charges** (28%)  
   - **Contract Type** (15%)  
   - **Payment Method** (5%)  



---

## 📢 Results & Business Recommendations  

🚀 **Key Takeaways:**  
✅ **Customers with long-term contracts churn less.**  
✅ **Fiber optic internet users have the highest churn rate.**  
✅ **Electronic check payment users are more likely to churn.**  

📌 **Recommendations for Neo Telecom:**  
✔ Offer **loyalty discounts** to long-term customers.  
✔ Incentivize customers to switch from **month-to-month contracts** to **annual plans**.  
✔ Improve **customer support** for fiber optic users to reduce dissatisfaction.  
✔ Provide **discounts or alternative payment options** for electronic check users.  

---

## 📍 Future Enhancements  

🔹 **Hyperparameter tuning** for Random Forest & Decision Tree models.  
🔹 Deploy a **web-based churn prediction tool** for real-time customer insights.  
🔹 Explore **Deep Learning models (ANN, CNN)** for better predictions.  
🔹 Implement a **customer retention strategy dashboard** using Power BI.  

---

## 📞 Contact  

👨‍💻 **Abhay Katiyar**  
📧 Email: (kumarabhaykatiyar@gmail.com)  
📌 GitHub: [GitHub Profile](https://github.com/kumarabhay03)  

---

🚀 **If you found this project insightful, drop a ⭐ on the repository!**  
