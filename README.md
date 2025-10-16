## End to End Machine Learning project 
# 📊 Telco Customer Churn Prediction

![Project Banner](churn.jpeg) ## 📖 Overview

This project aims to predict customer churn for a fictional telecommunications company. By analyzing customer data, we build a machine learning model that can identify customers who are likely to cancel their subscriptions. This predictive capability allows the company to proactively offer incentives and improve services to retain valuable customers.

The primary goal is to build a classification model with high accuracy and interpretability to understand the key drivers of churn.

----

## 🛠️ Tech Stack & Libraries

* **Python**
* **Pandas:** For data manipulation and analysis.
* **NumPy:** For numerical operations.
* **Scikit-learn:** For data preprocessing, modeling, and evaluation.
* **Matplotlib & Seaborn:** For data visualization.
* **Jupyter Notebook:** For interactive development and analysis.

----
## 📈 Model Performance & Results

The final model Random Forest Classifier was evaluated on the test set. Here are the key performance metrics:

* **Accuracy:** 100%
* **Precision:** 100%
* **Recall:** 100%
* **F1-Score:** 100%

### Confusion Matrix

The confusion matrix below visualizes the performance of our model. It shows the number of correct and incorrect predictions for both churn and non-churn classes.


*(This is a placeholder. Replace it with the image generated from your code.)*

|                | **Predicted: No Churn** | **Predicted: Churn** |
| :------------- | :---------------------- | :------------------- |
| **Actual: No Churn** | 1035 (TN)               | 0 (FP)              |
| **Actual: Churn** |   0 (FN)                | 374 (TP)             |

* **True Positives (TP):** 374 customers correctly identified as churners.
* **True Negatives (TN):** 1035 customers correctly identified as non-churners.
* **False Positives (FP):** 0 customers incorrectly identified as churners.
* **False Negatives (FN):** 0 actual churners were missed by the model.

### Top 15 Most Important Features

Feature importance analysis was conducted to identify the key drivers of customer churn. The chart below shows the top 15 features that had the most influence on the model's predictions. **Contract type**, **tenure**, and **monthly charges** are significant predictors.



Here is the list of the top 15 features:

1.  **Churn Value**
2.  **Churn Score**
3.  **Tenure Months**
4.  **Total Charges**
5.  **InternetService_Fiber optic**
6.  **Payment Method_Electronic check**
7.  **Monthly Charges**
8.  **Contract_Two year**
9.  **Dependents**
10. **CLTV**
11. **Streaming Movies_No Internet Service**
12. **Contract_One Year**
13. **Online Security_Yes**
14. **Tech Support_Yes**
15. **Internet Service_No**

---

## 🏁 Conclusion

The model demonstrates strong predictive power in identifying customers at risk of churn. The feature importance analysis reveals that customers on **month-to-month contracts**, with **low tenure**, and using **fiber optic internet service** are more likely to churn.

**Next Steps:**
* Deploy the model as a REST API for real-time predictions.
* Experiment with other advanced models like LightGBM or CatBoost.
* Gather more data to further improve model accuracy.