## **Income Prediction**

### **Objective**
Develop a predictive model to estimate a client’s monthly income (in UYU) based on financial and behavioral variables, minimizing the mean absolute percentage error (MAPE).

### **Problem Description**
The dataset includes information on current and past-due balances, contingencies, credit ratings, number of reporting financial institutions, and demographic variables.  
The objective is to capture complex relationships among these variables to accurately predict monthly income.

### **Methodology**
Multiple modeling approaches were evaluated, starting with baseline models and progressing toward more advanced techniques.  
The process included:

- Exploratory data analysis (EDA)
- Missing value imputation (KNN Imputer and Iterative Imputer)
- Outlier handling using Z-score
- Feature transformation and preparation
- Hyperparameter optimization through cross-validation
- Performance comparison across different models

The final model selected was **XGBoost**, due to its superior performance in terms of MAPE and its ability to capture non-linear relationships.

### **Evaluation**
The evaluation metric used was **mean absolute percentage error (MAPE)**.  
The XGBoost-based model showed solid performance on the validation set, achieving a MAPE close to **12%**, outperforming the defined benchmarks.

### **Results**
The trained model was used to generate predictions on the test set.  
Final results were exported to a CSV file containing the predicted monthly income values.

### **Conclusion**
The combination of robust preprocessing, iterative imputation, outlier handling, and hyperparameter optimization enabled the development of an accurate and stable income prediction model.

### **Note**
Due to confidentiality reasons, the datasets used for training and evaluation are not included in this repository.  
The code allows full reproduction of the modeling pipeline using local data.
