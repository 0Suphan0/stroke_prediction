
# Comparison of Machine Learning and Deep Learning Techniques for Stroke Prediction 

# Abstract
The early diagnosis and management of diseases in medicine have become critically important in today's world. This comparative thesis focuses on evaluating models developed using various machine learning and deep learning techniques (Logistic Regression, Decision Trees, Random Forest, Support Vector Machine, CNN 1-D, LSTM 1-D, BİLSTM 1-D) to determine the risk of stroke. The  obtained highest accuracy values are as follows: LR (0.96), DT (0.95), RF (0.95), SVM (0.96), CNN (0.9442), LSTM (0.9442), BİLSTM (0.9442). The study analyzes a dataset containing various clinical parameters (age, gender, hypertension, heart disease, marital status, occupation type, residence type, average glucose level, BMI, and smoking) using the healthcare-dataset-stroke-data/Fedesoriano. This comparative research aims to make a significant contribution to the field of health by evaluating the effectiveness of different machine learning and deep learning models in determining the risk of stroke.



# Dataset


## Dataset Properties
The data set used contains 5510 data and includes individuals with the following characteristics:
https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset

| id | Gender | Age | Hypertension | Heart Disease | Marital Status  | Occupation | Residence Type | Average Glucose Level | Body Mass Index | Smoking Status | Stroke |
|--------|----------|-----|---------------|-----------------|----------------|---------|--------------|---------------------------|---------------------|---------------------|-----|
| 1      | Male    | 45  | 0             | 1               | No          | Private    | City        | 87.5                      | 28.3                | have smoked before  | 0   |
| 2      | Female    | 35  | 1             | 0               | Yes           | Government  | Rural       | 110.2                     | 32.1                | never smoked       | 1   ||
| ...    | ...      | ... | ...           | ...             | ...            | ...     | ...          | ...                       | ...                 | ...               | ... |




  
# Methods

**Machine Learning:** Logistic Regression, Decision Trees, Random Forest, SVM

**Deep Learning:** CNN 1-D, LSTM, Bi-LSTM

# Results

**1-) Accuracy Values at Different Testing and Training Rates** 

| Accuracy                   | Logistic Regression | Decision Tree | Random Forest | SVM    |
|----------------------------|---------------------|---------------|---------------|--------|
| 10% Test - 90% Training     | 0.9491              | 0.8884        | 0.9491        | 0.9491 |
| 20% Test - 80% Training     | 0.9500              | 0.9080        | 0.9540        | 0.9559 |
| 30% Test - 70% Training     | 0.9562              | 0.9145        | 0.9543        | 0.9562 |
| 50% Test - 50% Training     | 0.9495              | 0.9021        | 0.9487        | 0.9495 |


**2-) Accuracy Values Changing According to Outliers** 

| Accuracy Values                                       | Logistic Regression | Decision Tree | Random Forest | SVM    |
|-------------------------------------------------------|--------------------|-------------|-----------------|--------|
| Before Removing Outliers                              | 0.9491             | 0.8884      | 0.9491          | 0.9491 |
| After Removing Outliers                               | 0.9557             | 0.9305      | 0.9578          | 0.9578 |
| Taking Mean of Outliers for the Dataset               | 0.9491             | 0.8884      | 0.9491          | 0.9491 |

**3-) Accuracy Values After Applying Lasso and PCA** 

| Accuracy Values     | Logistic Regression | Decision Tree Model | Random Forest Model | SVM    |
|----------------------|----------------------|----------------------|-----------------------|--------|
| Accuracy 1           | 0.9557               | 0.9305               | 0.9578                | 0.9578 |
| Accuracy 2 (LASSO)   | 0.96                 | 0.95                 | 0.95                  | 0.96   |
| Accuracy 3 (PCA)     | 0.9586               | 0.9158               | 0.9579                | 0.9586 |

**4-) Ensemble Learning Accuracy Values** 


| Ensemble                        | Accuracy Values |
|---------------------------------|----------------|
| LR, DT, RF, SVM                  | 0.9585         |
| LR, DT, RF, SVM, with LASSO       | 0.96           |
| LR, DT, RF, SVM, with PCA         | 0.9586         |
| CNN, LSTM, BiLSTM               | 0.9442         |

**5-) Accuracy Values Varying at Different Epoch Values** 

|        | CNN    | LSTM   | BiLSTM |
|--------|--------|--------|---------|
| Epoch-10| 0.9431 | 0.9442 | 0.9421  |
| Epoch-50| 0.9442 | 0.9442 | 0.9442  |

**6-) Accuracy Values of Hybrid Models in Deep Learning Algorithms** 

| Model             | Accuracy Value |
|-------------------|----------------|
| CNN, LSTM         | 0.9442         |
| CNN, BiLSTM      | 0.9442         |
| CNN, LSTM, BiLSTM | 0.9442         |

## Conclusion

In this study, the effectiveness of machine learning and deep learning algorithms used for stroke prediction was comprehensively evaluated and the accuracy rates between various models were compared. According to the research results, machine learning algorithms such as Logistic Regression, Support Vector Machines, Random Forest, Decision Trees and deep learning algorithms such as Convolutional Neural Network, Long-Short Term Memory and Bidirectional Long Short Term Memory have significant potential in stroke prediction. Additionally, dimension reduction techniques such as Lasso and Principal Component Analysis (PCA) and Ensemble Learning methods were used to increase the accuracy and generalizability of the model. As a result of the studies, the highest accuracy rate was obtained in the post-LASSO, Logistic Regression, post-LASSO Support Vector Machines and Machine Learning Algorithms Ensemble Learning (LR, KA, RO, SVM) method, with an accuracy rate of 0.96.
