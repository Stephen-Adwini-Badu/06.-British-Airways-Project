# British Airways Project 

## Project Overview
This project focuses on developing a machine learning classification model to predict customer behavior, specifically distinguishing between customers who successfully book flights and those who cancel. By leveraging data analysis techniques, the project aims to improve decision-making and enhance customer retention strategies for British Airways.

---

## Objectives
- Develop a classification model to predict customer booking outcomes.
- Analyze customer data to identify trends and insights.
- Use advanced machine learning techniques to improve model performance.

---

## Methodology
### 1. **Importing Libraries**
   - Utilized essential libraries such as Pandas, NumPy, Matplotlib, Seaborn, and Scikit-learn for data analysis and machine learning.

### 2. **Exploratory Data Analysis (EDA)**
   - Analyzed data to understand customer booking patterns.
   - Investigated missing values, data distributions, and correlations.

### 3. **Data Visualization**
   - Created visualizations to identify trends and relationships.
   - Plotted charts including histograms, bar plots, and scatter plots.

### 4. **Data Preparation**
   - Balanced imbalanced datasets to ensure model fairness.
   - Split data into training, validation, and testing datasets.

### 5. **Model Development**
   - Implemented multiple tree-based classifiers.
   
### 6. **Model Evaluation**
- Although the performance differences between the models are relatively small, Gradient Boosting has a slight edge in terms of accuracy, precision, recall, and F1 score.
     1. Similar Accuracy: Gradient Boosting and X Gradient Boosting have the same accuracy (79.0%), which is slightly higher than Random Forest (77.0%).

     2. Low Precision and Recall: All models have relatively low precision and recall values, indicating that they struggle to accurately predict the positive class.

     3. Gradient Boosting has Slightly Better F1 score: Gradient Boosting has a slightly higher F1 score (24.0%) compared to Random Forest (22.0%) and X Gradient Boosting (20.0%).

     4. Similar ROC AUC: All models have similar ROC AUC values, ranging from 54.0% to 55.0%.

<table align="center">
 <tr>
    <th>MODEL</th>
    <th>ACCURACY</th>
    <th>PRECISION</th>
    <th>RECALL</th>
    <th>F1 SCORE</th>
    <th>ROC-AUC</th>
 </tr>
 <tr>
    <td>Random Forest Classifier</td>
    <td align="center">77.0%</td>
    <td align="center">23.0%</td>
    <td align="center">21.0%</td>
    <td align="center">22.0%</td>
    <td align="center">54.0%</td>
 </tr>
 <tr>
    <td>Gradient Boosting Classifier</td>
    <td align="center">79.0%</td>
    <td align="center">25.0%</td>
    <td align="center">22.0%</td>
    <td align="center">24.0%</td>
    <td align="center">55.0%</td>
 </tr>
 <tr>
    <td>X Gradient Boosting Classifier</td>
    <td align="center">79.0%</td>
    <td align="center">23.0%</td>
    <td align="center">18.0%</td>
    <td align="center">20.0%</td>
    <td align="center">54.0%</td>
 </tr>
</table>

- **ROC-AUC and Calibration Curves**
    - **ROC Curve:** The AUC values for all three models (RFC, GBC, XGB) are close to 0.5, suggesting poor discrimination ability. This means that the models are not effective in distinguishing between the positive and negative classes.

    - **Calibration Curve:** The calibration curves show that the predicted probabilities are not well-calibrated, as they deviate from the perfect calibration line. This indicates that the models' predicted probabilities do not accurately reflect the true likelihood of the positive class.

 Overall, the performance of all three models is suboptimal, with poor discrimination ability and inaccurate probability predictions. This suggests that these models may not be reliable for this particular classification task.

![6 1](https://github.com/user-attachments/assets/ed3cffe2-68e5-4efb-ae46-0c3e274f3d7b)
     
- **Confusion Matrices** 
    - **The X Gradient Boosting Model** demonstrates the **best performance** in predicting bookings, with the highest percentage of correctly predicted "Booked" cases (76%) and the lowest percentage of incorrectly predicted "Cancelled" cases (8.8%).

    - **All models** have similar rates of **incorrectly predicting** "Cancelled" cases as "Booked" **(12%).**

    - **The X Gradient Boosting Model** also has the **highest percentage of correctly predicted "Cancelled" cases (2.6%)**, indicating a slight edge over the other models in terms of accuracy and reliability for both classes.

![6 1](https://github.com/user-attachments/assets/5f401578-ef75-4679-9b78-6d49e79dd891)

**Feature Importance**
- With regards to feature importance the most consistently influencial feature was **Flight Duration**  
- Another notable feature was;  
  - **In Flight Meals**  

![Image](https://github.com/user-attachments/assets/947297b4-c852-4f33-89e7-da966c6accfe)
