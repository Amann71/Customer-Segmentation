This project involves customer segmentation using the Mall_Customers.csv dataset. The Jupyter Notebook (CustomerSegmentationn.ipynb) applies clustering algorithms to categorize customers based on demographics and spending behavior. It’s an insightful exercise for understanding customer behavior, useful in targeted marketing and business strategy.

Table of Contents

Project Overview
Dataset
Data Preprocessing
Model Building
Model Evaluation
Visualizations
Conclusion
How to Run
Requirements
Contact
Project Overview

The main objective of this project is to perform customer segmentation by analyzing their demographics and purchasing behavior. The analysis includes:

Data import and preprocessing
Outlier detection and removal
Model building using linear and logistic regression
Visualization of customer data and model outcomes
Evaluation of the model's performance
Dataset

The dataset used in this project is a mall customer dataset, which contains the following columns:

CustomerID: Unique identifier for each customer
Gender: Gender of the customer
Age: Age of the customer
Annual Income (k$): Annual income of the customer in thousands of dollars
Spending Score (1-100): Score assigned by the mall based on customer behavior and spending nature
Data Preprocessing

Handling Missing Values: The dataset was cleaned by removing any missing values.
Categorical Encoding: The 'Gender' column was converted to numerical values using Label Encoding.
Outlier Detection and Removal: Outliers were identified using the IQR method and removed to ensure the quality of the data.
Feature Scaling: The features Age, Annual Income (k$), and Spending Score (1-100) were scaled using StandardScaler for better model performance.
Dropping CustomerID: The CustomerID column was dropped as it does not contribute to the predictive model.
Model Building

Logistic Regression:

Objective: Classify customers into two categories based on whether their spending score is above or below the average.
Model Performance: Evaluated using accuracy score and confusion matrix.
Model Evaluation

Logistic Regression: Achieved an accuracy of approximately 75%, indicating decent performance in classifying customers.
Visualizations

Scatter Plot: Visualized the relationship between Age and Spending Score.
Correlation Heatmap: Displayed correlations among different features.
Boxplot: Used to visualize the distribution of Annual Income (k$) after outlier removal.
Conclusion

The customer segmentation project effectively identified patterns in customer behavior. The analysis highlights that while age has some influence on spending score, other factors like income and gender also play a role. The models provide a good starting point for predicting customer spending patterns, but further refinement could improve accuracy.

How to Run

Clone the repository:
   git clone https://github.com/deependraxx/Customer-Segmentation-Project.git
Navigate to the project directory:
   cd Customer-Segmentation-Project
Install the required libraries:
   pip install -r requirements.txt
Run the Jupyter Notebook to see the analysis:
   jupyter notebook Customer_Segmentation.ipynb
Requirements

1.Python 3.7 or above 2.pandas 3.numpy 4.matplotlib 5.seaborn 6.scikit-learn 7.scipy
