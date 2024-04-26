**BMI PREDICTION PROJECT:**

This project aims to predict Body Mass Index (BMI) using machine learning techniques. BMI is a measure of body fat based on height and weight that applies to adult men and women. The prediction is made using features such as age, height, weight, and sex.


**LITERATURE REVIEW:**

As a foundational step in this project, we conducted a literature review to understand existing approaches and findings related to BMI prediction. The process involved selecting and analyzing four research papers focusing on BMI prediction methods and outcomes. Key steps of the literature review process are outlined below:-

**1. Selection of Research Papers:** We identified and selected four research papers from reputable journals and conference proceedings, each addressing different aspects of BMI prediction. The selected papers covered topics such as feature selection, machine learning algorithms, demographic factors, and health implications of BMI.

**2. Literature Analysis:** We thoroughly reviewed each paper, paying close attention to the methodologies employed, datasets used, features considered, and predictive performance metrics reported. Additionally, we analyzed the problem statements addressed in each paper and the conclusions drawn by the authors.

**3.Identifying Common Themes and Challenges:** Through the literature review, we identified common themes, trends, and challenges in BMI prediction research. This process helped us gain insights into the state-of-the-art techniques, potential limitations, and areas for improvement in existing approaches.

**4.Formulation of Problem Statement:** Based on the findings of the literature review, we formulated a clear problem statement for our project, highlighting the need to develop a robust BMI prediction model that accounts for diverse demographic factors and utilizes advanced machine learning techniques.

**5.Conclusion:** The literature review concluded with a synthesis of key insights gleaned from the analyzed papers, along with recommendations for future research directions. This informed our approach to designing and implementing the BMI prediction project, ensuring that it builds upon existing knowledge while addressing identified gaps and challenges.


**METHODS COMPARISON:**

**Method 1: Dropping Null Values**
In this method, null values in the dataset are dropped, and linear regression modeling is applied to predict BMI based on height and weight data. After preprocessing, a heatmap of the dataset is generated and compared with Method 2.

**Method 2: Filling Null Values with Central Tendencies**
This method involves more advanced techniques such as filling null values with central tendencies (mean, median, mode). After preprocessing, including encoding sex columns using one-hot encoder and scaling the data values using standard scaler, a heatmap of the dataset is generated and compared with Method 1.

**HEATMAP COMPARISON:**

After comparing, it was found that the heatmaps of both methods are the same.

**DATA PREPROCESSING:**

After comparing the heatmaps, the next step was data preprocessing. This involved the following steps:

1.Renaming the column headers.

2.Encoding the sex column using one-hot encoding.

3.Separating the target column from the source data to compare with the predictions later.

4.Scaling the data values using standard scaler.

5.Splitting the data into training and testing sets.

6.Creating a Predictive Data model using XGBRegressor.


Once the data preprocessing was completed, a predictive data model was created using XGBRegressor. This model was trained on the preprocessed data to predict BMI based on the selected features.

Cross-Validation
Cross-validation was performed using the XGBoost model on the 'newData' features and 'target' values with 5-fold cross-validation. The cross-validation scores were [0.99873248, 0.99895118, 0.99872162, 0.99865727, 0.99880439], with a mean score of 0.9987733870124897.

Model Evaluation
Predictions were made using the trained XGBoost model on the test data (xtest), yielding R-squared scores of 0.998825558006925. The predictions were consistent with the actual 'ytest' values, demonstrating the model's accuracy.

Health Status Prediction
Predictions were made using the trained XGBoost model on the 'newData' features, resulting in an array of predicted BMI values. These predicted values were categorized into health statuses based on BMI ranges, including 'Underweight', 'Normal', 'Overweight', 'Obese', and 'Extremely Obese'.
