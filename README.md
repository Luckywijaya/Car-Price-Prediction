# Car-Price-Prediction
Make a regression predictive model to predict the car price.

# Project Overview

• Seek insight from the dataset with Exploratory Data Analysis <br>
• Performed data cleansing, data processing, data engineering to prepare data before modeling<br>
• Built a model to predict the car price<br>
<br>
# Exploratory Data Analysis
| Variable | Type | Definition |
| ----------- | ----------- | ----------- |
| id | Numeric | Unique car ID 
| symbol | Categorical | Assigned insurance risk rating (+3 is risky, -3 is safe)
| name | Categorical | Name of car company |
| fuel | Categorical | Car fuel type |
| aspiration | Categorical | Aspiration used in a car |
| door | Categorical | Number of doors |
| body | Categorical | Body of car |
| wheel | Categorical | Type of drive wheel |
| engineloc | Categorical | Location of car engine |
| wheelbase | Numeric | Wheelbase of car |
| length | Numeric | Length of car |
| width | Numeric | Width of car |
| height | Numeric | Height of car |
| weight | Numeric | Weight of a car without occupants or baggage |
| engine | Categorical | Type of engine |
| cylinder | Categorical | Cylinder number placed in the car |
| enginesize | Numeric | Size of car |
| fuelsystem | Categorical | Fuel system of car |
| boreratio | Numeric | Boreratio of car |
| stroke | Numeric | Stroke or volume inside the engine |
| compressionratio | Numeric | Compression ratio of car |
| hp | Numeric | Horsepower |
| peakrpm | Numeric | Car peak rpm |
| citympg | Numeric | Mileage in city |
| highwaympg | Numeric | Mileage on highway |
| price | Numeric | Price of car |

<br><br>
![image](https://user-images.githubusercontent.com/80570935/129027678-c2e7e7c6-bc9c-40eb-9eec-8f2eee109d59.png)
There are outliers in `wheelbase`, `with`, `enginesize`, `stroke`, `compressionration`, `hp`, `peakrpm`, `highwaympg`, and `price`. <br>
Overall the features has normal distribution. 
<br><br>
![image](https://user-images.githubusercontent.com/80570935/129028368-b4365d95-c507-43fe-a578-f22e97a776aa.png)
Based on `fuel`, `door`, `body`, `wheel`, `engine`, `cylinder` features, majority is a city cars. <br>

# **Data Processing**<br>
• Check missing & duplicate values<br>
• Replace all features that have an outliers with IQR limit<br>
• Ordinal encoding for `door` & `cylinder` features<br>
• Feature encoding the rest of categorical columns<br>
• Drop categorical features that encoded before<br>
• Normalize all selected features <br>
<br><br>
# **Modeling**<br>
• Split features & target<br>
• Split data into data train & data test<br>
• Train model with 4 different algorithm such as Linear Regression, Random Forest, Decision Tree<br>
• Evaluate model with MAE Score, RMSE Score & R2 Score<br>
• Validate model with train and test accuracy <br>
• Hyperparameter tuning<br>
• Select the best model<br>
<br><br>
# **Model Evaluation**<br>
