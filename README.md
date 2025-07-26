House Price Prediction Using Linear Regression:

This project uses Linear Regression to predict house prices based on various features such as square footage, number of bedrooms/bathrooms, property age, and other housing characteristics.

Dataset:

->The dataset contains historical sales data with attributes like:

->Living area and lot size

->Year built and renovation year

->Building grade

->Location (zip code)

->Sale price (target)

Project Goals:

->Build a predictive model to estimate house sale prices.

->Engineer new features like house age and since renovation.

->Evaluate model performance using R² score and MSE.

->Visualize actual vs predicted prices.

->Make predictions for custom sample input.

Workflow & Methodology:

Data Preprocessing:

->Dropped irrelevant fields: id, date, DocumentDate, ym, PropertyType.

->Handled missing values with median imputation.

->Feature Engineering:

->house_age = 2025 - YrBuilt

->since_renovation = 2025 - YrRenovated (or 0 if never renovated)

Feature Scaling:

->Used StandardScaler to normalize numerical features before model training.

Model Building:

->Used LinearRegression from scikit-learn.

->Trained on 80% of the dataset, tested on 20%.

Evaluated with:

->Mean Squared Error

->R² Score

Visualization:

Scatter plot of actual vs predicted prices using Seaborn.

Sample Prediction:

A test house is manually defined and passed to the model for prediction.

Libraries Used:

->pandas, numpy – for data manipulation

->matplotlib, seaborn – for visualization

->sklearn – for preprocessing, modeling, and evaluation
