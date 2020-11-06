**PREDICTING SELLING PRICES OF HOUSES IN SEATTLE, USA**

W5 - PROJECT

**Background**: For a real estate company, build a machine learning model to predict the selling prices of houses based on a variety of features on which the value of the house is evaluated.

**Objective**: The task is to build a model that will predict the price of a house based on features provided in the dataset. The senior management also wants to explore the characteristics of the houses using some business intelligence tool. One of those parameters include understanding which factors are responsible for higher property value - \$650K and above.

**Data**: The data set consists of information on some 22,000 properties.  The dataset consisted of historic data of houses sold between May 2014 to May 2015.

**Methodology**: The dataset was first imported into MySQL and an initial data exploration was done by means of SQL queries. After having a clear overview, the dataset was imported to Jupyter Notebook by establishing the connection with MySQL. After an initial check for NA and Null values, we divided the data into numerical and categorical. Using the method describe on numerical columns I got a numerical overview of the dataset. We then plotted a 'Pearson' Correlation Matrix to check the correlation between the features of the dataset. 

While checking for outliers, we saw a potential problem with outliers limiting the predictive power of the model. We checked the distributions of continuous variables by using matplotlib and seaborn, and found that all variables were positively skewed, so we transformed the data. This improved the distributions dramatically. The next step was to dummify categorical columns and concatenate the data. We went on to divide the data between the dependant and independant variables, and to split between train and test sets. We initially tried a Linear Regression Model, a KNN model, and a Decision Tree Regressor.


Model 2 - Ernesto
I got the best results with the linear regression and decided to stick with it (allowing my colleagues to work with the other models). I went back and did some feature engineering, creating a column to classify between houses with basement and houses without basement. I also dropped columns which I found irrelevant or highly correlated with other features. These two actions improved the model significantly.

Model 3 - Macarena
After doing feature engineering and classifying the houses, we were not able to increase further the performance of the model. I decided to run several models to predict the prices of the houses that were limiting the predictive power of our model. However, when conducting the predictions, our sample became smaller and smaller, the outliers were harder to predict and the overall model performance did not improve. I then attempted to classify the houses according to a location parameter, which if explored further could potentially lead to a better performance. 


