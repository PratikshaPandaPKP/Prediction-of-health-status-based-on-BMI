**BMI Prediction Project:**

This project aims to predict Body Mass Index (BMI) using machine learning techniques. BMI is a measure of body fat based on height and weight that applies to adult men and women. The prediction is made using features such as age, height, weight, and sex.


**Literature Review:**

As a foundational step in this project, we conducted a literature review to understand existing approaches and findings related to BMI prediction. The process involved selecting and analyzing four research papers focusing on BMI prediction methods and outcomes. Key steps of the literature review process are outlined below:-

**1. Selection of Research Papers:** We identified and selected four research papers from reputable journals and conference proceedings, each addressing different aspects of BMI prediction. The selected papers covered topics such as feature selection, machine learning algorithms, demographic factors, and health implications of BMI.

**2. Literature Analysis:** We thoroughly reviewed each paper, paying close attention to the methodologies employed, datasets used, features considered, and predictive performance metrics reported. Additionally, we analyzed the problem statements addressed in each paper and the conclusions drawn by the authors.

**3. Identifying Common Themes and Challenges:** Through the literature review, we identified common themes, trends, and challenges in BMI prediction research. This process helped us gain insights into the state-of-the-art techniques, potential limitations, and areas for improvement in existing approaches.

**4. Formulation of Problem Statement:** Based on the findings of the literature review, we formulated a clear problem statement for our project, highlighting the need to develop a robust BMI prediction model that accounts for diverse demographic factors and utilizes advanced machine learning techniques.

**5. Conclusion:** The literature review concluded with a synthesis of key insights gleaned from the analyzed papers, along with recommendations for future research directions. This informed our approach to designing and implementing the BMI prediction project, ensuring that it builds upon existing knowledge while addressing identified gaps and challenges.


**Methods Comparison:**

**Method 1: Dropping Null Values**
In this method, null values in the dataset are dropped, and linear regression modeling is applied to predict BMI based on height and weight data. After preprocessing, a heatmap of the dataset is generated and compared with Method 2.

**Method 2: Filling Null Values with Central Tendencies**
This method involves more advanced techniques such as filling null values with central tendencies (mean, median, mode). After preprocessing, including encoding sex columns using one-hot encoder and scaling the data values using standard scaler, a heatmap of the dataset is generated and compared with Method 1.

**Heatmap Comparison:**

After comparing, it was found that the heatmaps of both methods are the same.

**Data Preprocessing:**

After comparing the heatmaps, the next step was data preprocessing. This involved the following steps:

1. Renaming the column headers.

2. Encoding the sex column using one-hot encoding.

3. Separating the target column from the source data to compare with the predictions later.

4. Scaling the data values using standard scaler.

5. Splitting the data into training and testing sets.

6. Creating a Predictive Data model using XGBRegressor.


Once the data preprocessing was completed, a predictive data model was created using XGBRegressor. This model was trained on the preprocessed data to predict BMI based on the selected features.

**Cross-Validation:**

Cross-validation was performed using the XGBoost model on the 'newData' features and 'target' values with 5-fold cross-validation. The cross-validation scores were [0.99873248, 0.99895118, 0.99872162, 0.99865727, 0.99880439], with a mean score of 0.9987733870124897.

**Model Evaluation:**

Predictions were made using the trained XGBoost model on the test data (xtest), yielding R-squared scores of 0.998825558006925. The predictions were consistent with the actual 'ytest' values, demonstrating the model's accuracy.

**Health Status Prediction:**

Predictions were made using the trained XGBoost model on the 'newData' features, resulting in an array of predicted BMI values. These predicted values were categorized into health statuses based on BMI ranges, including 'Underweight', 'Normal', 'Overweight', 'Obese', and 'Extremely Obese'.

**Conclusion:**

Prediction of health status based on BMI can be improved with AI.
XGBoost is a highly effective regression algorithm that can make very accurate predictions.
This project can help the medical industry by predicting health status with high accuracy.
There is still room for improvement, as healthcare and AI are constantly evolving.

**Additional Context:**

Completed by me and my friend Amreen Kazi in October 2023 during our third semester in the MS in Data Science program as an assignment, this project represented the culmination of our collective efforts and academic endeavors. It served as a testament to our dedication, perseverance, and proficiency in the field of data science. As we reflect on this milestone achievement, completed within the structured framework of our MS program, we recognize the invaluable learning experiences, professional growth, and collaborative spirit fostered by our academic journey.

**Project Files Overview:**

**bmi_data.csv:** The dataset containing features for predicting Body Mass Index (BMI).

**Prediction_of_health_status_based_on_Body-Mass-Index.ipynb:** The Jupyter Notebook containing the Python code for data preprocessing, model building, evaluation, and prediction of BMI and health status categories.

**Literature Review, Problem Statement & Conclusion.pdf:** The report covering the literature review of four research papers, the formulated problem statement, and the project's conclusion.

**BODY MASS INDEX BDA Project PPT 02_09.pptx:** The PowerPoint presentation explaining the project's introduction, methodology, results, and findings.
