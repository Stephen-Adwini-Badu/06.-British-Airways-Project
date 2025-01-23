# British Airways Project Notebook

## Project Overview
This project focuses on developing a machine learning classification model to predict customer behavior, specifically distinguishing between customers who successfully book flights and those who cancel. By leveraging data analysis techniques, the project aims to improve decision-making and enhance customer retention strategies for British Airways.

---

## Objectives
- Develop a classification model to predict customer booking outcomes.
- Analyze customer data to identify trends and insights.
- Use advanced machine learning techniques to improve model performance.

---

## Methodology
1. **Importing Libraries**
   - Utilized essential libraries such as Pandas, NumPy, Matplotlib, Seaborn, and Scikit-learn for data analysis and machine learning.

2. **Exploratory Data Analysis (EDA)**
   - Analyzed data to understand customer booking patterns.
   - Investigated missing values, data distributions, and correlations.

3. **Data Visualization**
   - Created visualizations to identify trends and relationships.
   - Plotted charts including histograms, bar plots, and scatter plots.

4. **Data Preparation**
   - Balanced imbalanced datasets to ensure model fairness.
   - Split data into training, validation, and testing datasets.

5. **Model Development**
   - Implemented multiple tree-based classifiers.
   
6. **Model Evaluation**
   - Compared multiple classifiers and identified the best-performing model.
   - Validated models using precision, recall, F1 scores, and confusion matrices.

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

---

## Key Insights
- Comparison of various machine learning models highlighted the effectiveness of ensemble methods.
- Visualization of booking trends revealed actionable insights for customer management strategies.
- Identification of significant features impacting booking cancellations.

![Image](https://github.com/user-attachments/assets/947297b4-c852-4f33-89e7-da966c6accfe)

---

## Results
- Achieved high prediction accuracy using ensemble classifiers.
- Balanced models provided improved predictions for both successful bookings and cancellations.
- Confusion matrix analysis highlighted reduced false positives and improved precision.

---

## Conclusion
This project successfully developed a classification model that predicts customer booking behavior. The insights derived from the data analysis provide valuable guidance for enhancing customer service strategies at British Airways. Future work can explore integrating additional features and real-time data for further improvements.
