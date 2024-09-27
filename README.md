# House-Price-Prediction-Using-Machine-Learning
1.Aim - This project is focused on building a machine learning model to predict house prices in Bangalore, India. It involves several key steps, including data preprocessing, feature engineering, outlier removal, model selection, and deployment using Streamlit. The project aims to provide a practical solution for homebuyers, sellers, and real estate enthusiasts in estimating property prices. 

2.Dataset Description - This dataset contains information about residential properties in various locations, specifically focused on their characteristics and pricing. Each entry represents a unique property listing and includes the following columns: 
Location: The geographical area where the property is situated (e.g., Electronic City, Whitefield). 
Size: The type of property, typically categorized by the number of bedrooms or rooms (e.g., 2 BHK, 4 Bedroom). 
Total Sq Ft: The total area of the property measured in square feet (e.g., 1056.0 sq ft). 
Bath: The number of bathrooms in the property (e.g., 2.0). 
Price: The total selling price of the property in a currency unit (e.g., $39.07, indicating the price in thousands). 
BHK: The number of bedrooms, kitchen, and hall (e.g., 2, 3, 4), with "BHK" referring to a specific type of property layout. 
Price per Sq Ft: The price of the property per square foot, providing insight into the cost efficiency of the property (e.g., 3699.81).

3. Objectives: 
Data Collection: The dataset used for this project is obtained from Kaggle. It includes various features related to real estate properties in Bangalore, such as location, total square feet area, number of bedrooms (BHK), number of bathrooms, price, and more. 
Data Preprocessing: Initial data exploration to understand the dataset's structure and characteristics. Handling missing values by removing rows with missing data. 
Creating a new feature, "bhk," by parsing the number of bedrooms from the "size" feature. Cleaning the "total_sqft" feature by converting it into a numerical format. This involves handling ranges and non-standard entries. 
Creating a new feature, "price_per_sqft," to normalize prices based on square feet area. Dimensionality reduction by categorizing less frequent location values as "other" to reduce the number of categories. 
Outlier Detection and Removal: Removing outliers based on business logic, such as properties with low square feet per bedroom. 
Utilizing the mean and standard deviation to identify and remove price per square feet outliers for each location. Further refining the dataset by removing properties where the number of bathrooms exceeds the number of bedrooms plus two. 

4. Model Building and Selection: The Linear Regression model is chosen as the primary predictive model for this project. 
The dataset is split into training and testing sets for model evaluation. Cross-validation is applied to ensure model performance consistency. 
A GridSearchCV process is used to find the best hyperparameters for the selected models. Other models like Lasso and Decision Tree Regression are considered and evaluated for their performance. 
Streamlit Web App Development: A Streamlit web application is created to provide an interactive interface for users to predict house prices. Users can input location, total square feet, number of bedrooms, and number of bathrooms to get a price prediction. 
Model Deployment: The trained Linear Regression model is saved to a pickle file for use in the Streamlit app. The Streamlit app is set up to run locally and deployed on a web server for public access. This project can be a valuable resource for individuals looking to explore real estate trends and estimate property prices in Bangalore, India. 
It combines data science techniques, machine learning, and interactive web development to create a user-friendly tool for real estate analysis.
