# Laptop Price Prediction Model
## Problem Statement
The increasing variety and complexity of laptops in the market make it challenging for consumers to estimate the fair market price for a given set of laptop specifications. This project aims to develop a predictive model that accurately estimates the price of a laptop based on various features and specifications.
## Data Collection
To create an effective model, data collection was the first critical step. I downloaded a dataset from Kaggle, but it contained a small number of observations. Therefore, I tried gathering additional data from Amazon using the Beautiful Soup and Requests libraries.
<br><br>
    •	Beautiful Soup: A Python library for parsing HTML and XML documents. It creates parse trees from page source code, which can be used to extract data easily.<br><br>
    •	Requests: A simple-to-use HTTP library for making HTTP requests in Python. It simplifies sending requests and receiving responses, making it easier to scrape web data.
## Data Cleaning
The collected data was highly jumbled and required extensive cleaning. This included extracting information from cluttered columns and creating new, meaningful columns. For instance, I combined two columns representing resolution (X and Y) into one column, "PPI" (Pixels Per Inch).<br><br>
•	PPI (Pixels Per Inch): A measure of pixel density on a display, indicating how many pixels are packed into one inch of the screen.
## Data Visualization
Data visualization helped to understand the insights from the data. During this step, I discovered that the target variable (price) was skewed.<br><br>
•	np.log: A function from the NumPy library that applies the natural logarithm to the data. It is used to normalize skewed data, making it more suitable for modeling.
## Hypothesis Testing
I conducted hypothesis testing to validate assumptions about the data.<br><br>
•	Hypothesis Testing: A statistical method that helps in making inferences about the population based on sample data. It is advantageous as it provides a systematic way to test assumptions and validate models.

## Encoding and Splitting Data
Categorical data was converted into numerical format using encoding techniques, and the dataset was split into training and testing sets to build the model effectively.
## Model Building
I experimented with various regression models including Linear Regression, Ridge, Lasso, KNN, SVM, Decision Tree, Random Forest, AdaBoost, Gradient Boosting, and XGBoost. Initially, without hyperparameter tuning, I achieved an accuracy score of approximately 78%.
## Hyperparameter Tuning
For ensemble learning methods (Random Forest, AdaBoost, Gradient Boosting, XGBoost), hyperparameter tuning was performed to improve model performance.<br><br>
•	Evaluation Metrics: Used to assess the performance of the models, including MAE (Mean Absolute Error), MSE (Mean Squared Error), RMSE (Root Mean Squared Error), and R2 Score. XGBoost provided the best results among all models.<br><br>
•	After hyperparameter tunning I found out my XGBoost model giving me high accuracy.<br><br>
•	MAE = 0.13 ,  MSE = 0.03,  RMSE = 0.18 , R2 = 0.90  ,  Adjusted R2 = 0.90 
<br><br>
![image](https://github.com/zaid105/Laptop-Price-Prediction/assets/142628044/d42ce177-0f48-4e22-b5db-fa55396aa8f7)
## Dashboard:
•	With the help of ‘Power BI’ I created a beautiful dashboard.

## Deployment
The final step was to deploy the model so it can be used in real-world scenarios. Deployment involves making the model available to users through a platform or application.
This summary encapsulates the process of building a predictive model for estimating laptop prices based on specifications, from data collection to deployment.
<br><br>
Deployed on Render:
<br>Render is a cloud platform designed for developers to deploy and manage web applications, backend services, databases, and machine learning models.

## Risk And Challenges
In this project, I faced several challenges that made the analysis more complicated. Here are the main issues:<br><br>
1.	Small Dataset: The dataset had only 1300 rows and 12 columns. This small size made it difficult for the model to achieve high accuracy because there wasn't much data to learn from.<br><br>
2.	Feature Engineering: I had to do a lot of feature engineering, which means creating new columns from the existing data. This was necessary to gain a deeper understanding of the dataset. However, it was tricky to extract meaningful insights from these new features.<br><br>
3.	Complex Data Processing: Creating new columns based on the knowledge I acquired was challenging. Despite these difficulties, I kept working on the analysis to make the most out of the limited data and to extract valuable insights from the newly created features.
<br><br>

# User Interface
![Screenshot 2024-03-09 195551](https://github.com/zaid105/Laptop-Price-Prediction/assets/142628044/b6b0f3ca-79b2-4c7a-9774-26552325005d)


![Screenshot 2024-03-09 195620](https://github.com/zaid105/Laptop-Price-Prediction/assets/142628044/c9b32110-24d6-4b05-88ee-68b140bd416d)












