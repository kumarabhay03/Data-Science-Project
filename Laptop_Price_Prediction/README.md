## 💻 Laptop Price Prediction and Analysis

This project explores a dataset of laptop specifications and prices, performing an in-depth **Exploratory Data Analysis (EDA)** to uncover market trends and developing machine learning models to **accurately predict laptop prices**.

The work reveals key pricing factors, component distributions, and the superior performance of tree-based models over linear methods for this task.

***

## 📊 Dataset Overview

The dataset comprises **1275 entries** with **23 features** detailing laptop specifications, including manufacturer, CPU, GPU, storage, screen resolution, and the target variable, **Price in Euros**.

* **Integrity:** The dataset is fully complete with **no missing values**.
* **Target Variable:** $\text{Price\_euros}$ exhibits high variability, ranging from **$174$ € to $6,099$ €**.

***

## 🔍 Exploratory Data Analysis (EDA) Highlights

The analysis revealed significant market patterns and component biases:

### Market & OS Dominance
* **Companies:** The market is heavily dominated by a few major players: **Dell, Lenovo, and HP** account for the vast majority of devices.
* **Operating System (OS):** Over **$80\%$** of devices run **Windows 10**, confirming a highly focused market.

### Hardware & Configuration
* **RAM:** The most common RAM size is **$8$ GB** (the standard for mid-range), followed by $4$ GB and $16$ GB.
* **CPU/GPU:** The dataset is almost exclusively ($\approx 95\%$) powered by **Intel** processors, often paired with Intel's integrated graphics.
* **Storage:** The primary storage standard is **$256$ GB SSD**. Critically, over **$85\%$** of devices **do not include secondary storage**.

### Price Drivers (Key Relationships)
* **RAM vs. Price:** Price increases sharply with RAM, especially beyond $16$ GB. The most price-volatile configurations are those around $32$ GB.
* **Resolution vs. Price:** There is a clear, step-wise price premium for higher screen resolutions, progressing smoothly from Standard to Full HD, Quad HD+, and 4K Ultra HD.
* **Touchscreen Premium:** Touchscreen capability adds a price premium, especially for lower-resolution models, but this premium becomes negligible at the 4K Ultra HD level.
* **Manufacturer Price Stratification:** Prices are heavily stratified by company, with certain manufacturers (e.g., those represented by Company 14 in the box plots) consistently occupying the highest price brackets.

***

## 🧠 Modeling & Prediction

The project implemented and evaluated two common regression models to predict laptop price based on specifications.

### Model Performance Comparison

| Metric | Linear Regression | **Random Forest** |
| :--- | :--- | :--- |
| **$R^2$ Score** | $74.45\%$ | **$87.33\%$** |
| **MAE (Mean Absolute Error)** | $266.63$ € | **$156.70$ €** |
| **RMSE (Root Mean Squared Error)** | $363.83$ € | **$256.25$ €** |

### Conclusion

The **Random Forest** Regressor significantly outperformed the Linear Regression model, achieving an **$R^2$ score of $87.33\%$**. This confirms that the relationship between a laptop's specifications and its price is **highly non-linear** and is best captured by ensemble methods.

The Random Forest model predicts prices with an average absolute error of only **$\approx 157$ €**, making it highly accurate for real-world price estimation.

***

## 🛠️ Technologies Used

* **Python**
* **Pandas & NumPy** (Data Manipulation)
* **Matplotlib & Seaborn** (Data Visualization)
* **Scikit-learn (sklearn)** (Machine Learning Modeling)
