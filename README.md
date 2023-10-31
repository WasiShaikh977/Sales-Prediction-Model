# Sales-Prediction-Model
### Project Overview
In this study, the primary objective was to develop a machine learning and deep learning model that leverages historical sales data of similar products to predict the sales of unsold items.

We had data from a chain of stores selling food items. The data was divided into 2 datasets - 
- Train data (historical data with target column)
- Test data (Prediction dataset with no target column)

  ![](https://github.com/WasiShaikh977/Sales-Prediction-Model/blob/main/DL_RMSE.png)

### Resources
**Python Version:** 3.11


**Packages:** pandas, matplotlib, seaborn, numpy, sklearn, tensorflow, plotly, scipy

### Data Acquisition
- Data downloaded form kaggle and uploaded via a .csv file onto Jupyter notebook

### Data Cleaning, Exploration and Visualisation
- Carefully examined each column in the data to look for outliers, trends and patterns.
- Removed outliers from the visibility column.
- Deleted 2 columns which contained a high % of null values.
- Visualised and noted down the trends and patterns observed in the data.

### Machine Learning Models
- Used sklearn library to import 5 ML models and fit them to our dataset.
- Trained the data on Linear Regression, Ridge Regressoin, Lasso Regression, Random Forest Regressor and Gradient boosted Decision Tree.
- Used GridSearchCV to optimize the Random Forest model.

### Deep Leearning
- Trained 2 deep learning models on our data using the tensorflow library

### Model Performance
The Deep Learning model turned out to be out best model with an RMSE of 1074.7. Both the deep learning models were identical in their performance.
The top 3 models were as follows:
1 - Deep Learning: RMSE 1074.7
2 - Optimized Random Forest Regressor: RMSE 1077.5
3 - Gradient Boosted Decision Tree: RMSE 1082.5

### Conclusion
In this study, we used food products data from a chain of stores to build a sales prediction model. Even though the model is not as accurate as we like, we now have a framework to build upon and eventually find a model that is deployable in the real world. We can go about this in many ways, some of which include:
- Adding new variables in our data collection stage (Promotion, day of week, month, holiday period, etc)
- Hypertuning our models even further and trying out more ML models on the same data.
- Ensuring the data is entered correctly so we dont have to delete columns like Outlet size and product weight.

That said, the exploratoty data analysis helped us find some interesting insights.


#### Key Insights
1) Outlet **OUT027** is making the most amount of money.
2) Outlet location tier 3 seem to make the most sales. Especially the combination of Tier 3 location and SuperMarket Type 3.
3) Starchy foods and Dairy have high MRPs whereas Seafood and Starchy food seem to be making more sales on average.
4) Grocery Stores have been the worst performers compared to all other supermarket types.
5) Medium sized stores make the most amount of money followed by High and then Small. The mean MRP of the goods sold is nearly the same for all the sizes.
