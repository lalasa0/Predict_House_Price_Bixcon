1. Data Loading and Preprocessing:

> Load Data: The dataset is loaded from a CSV file using pandas.
> Handle Missing Values: Missing values are imputed in numerical columns with the mean and in categorical columns with the most frequent value.
> Feature and Target Definition: The dataset is split into feature (X) and target (y) variables.
    
2. Data Transformation:

> Preprocessing: Numerical features are standardized, and categorical features are one-hot encoded. This is done using ColumnTransformer with SimpleImputer and StandardScaler for numerical data, and OneHotEncoder for categorical data.
    
3. Model Training and Evaluation:

> Data Splitting: The data is split into training and testing sets (80% train, 20% test).
> Decision Tree Model: A DecisionTreeRegressor is trained and evaluated on the test set. Mean Squared Error (MSE) is calculated.
> Random Forest Model: A RandomForestRegressor is trained and evaluated similarly. MSE is calculated.
> Gradient Boosting Model: A GradientBoostingRegressor is trained and evaluated, with MSE calculated.
    
4. Cross-Validation:

> Decision Tree: Cross-validation is performed to compute the mean MSE using 5-fold cross-validation.
> Random Forest: Similar cross-validation is performed for the Random Forest model.
> Gradient Boosting: Cross-validation is performed for the Gradient Boosting model.
 
5. Visualization:

> Scatter Plot: A scatter plot can be created to compare actual vs. predicted values for Linear Regression, though this part is commented out.
