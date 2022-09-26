# Seoul-Bike-Sharing-Demand-Prediction

##   This project will be explored over the previous data in order to predict the number of bikes that can be rented per hour by the company. So that customers can get the best experience without any delays. We will build different regression models and check which proves to be the best for the deployment.

#### Tags: Regression, Python, Machine Learning, Data Science 

#### Team Members are: Rajesh kumar, Kunika Gupta, Prayagraj Dubey, Shivank Dueby and Parul Sharma

#### Links:  
Project Presentation: [Slideshow](https://drive.google.com/file/d/1HFd9jKPJBAGv-kOcDQg7HAqhuAMd0T4k/view?usp=sharing)
Dataset: [Bike Sharing Demand Prediction](https://drive.google.com/file/d/1A81TMIl0oe2G3SQ8zpT0AFJJtsZ26KAj/view?usp=sharing)

## Content:
The data are downloaded from the South Korean website named SEOUL OPEN DATA PLAZA. One-year data are used in this research. The period of the dataset is 365 days (12 months) from December 2017 to November 2018. From the data, the count of the rental bikes rented at each hour is calculated.

<h2><b>Steps involved doing this project</b></h2>

<h3><b>Loading and discovering data:</b></h3> Here, we need to load our data from the external source, which in this case is uploaded to the drive. The data is in the format of the CSV (Comma Separated Values) file.

<h3><b>Data Cleaning  and Null values treatment:</b></h3> Data cleaning is an important step in the data analytics process in which you either remove or update information that is incomplete or improperly formatted.  Null values Treatment by different methods. We have our dataset in hand which is raw and unfiltered. This step involves cleaning our data first by eliminating the columns which are not needed for our analysis. We have around 8760 rows × 14 columns in our dataset.Since, there were no null values, we have left it untouched.

<h3><b>Exploratory Data Analysis:</b></h3>Exploratory Data Analysis is the approach of analyzing data, gathering and summarizing the important characteristics of the information, and using simple visualization that makes it easier to understand.

<h3><b>Importing necessary modules and libraries:</b></h3>We are importing the following libraries for their respective applications:

 <h4><b>Pandas:-</h4></b> Pandas is used to analyze data. It has functions for analyzing, cleaning, exploring, and manipulating data.
 <h4><b>Matplotlib:-</h4></b>  Matplotlib is a graph plotting library in python that serves as a visualization utility. Most of the Matplotlib utilities lie under the pyplot submodule.
 <h4><b>Numpy:-</h4></b>  NumPy is a Python library used for working with arrays. It also has functions for working in the domain of linear algebra, Fourier transform, and matrices.
 <h4><b>SciKit:-</h4></b>  Scikit-learn (Sklearn) is the most useful and robust library for machine learning in Python. It provides a selection of efficient    tools for machine learning and statistical modeling including classification, regression, clustering and dimensionality reduction via a consistent interface in Python. This library, which is largely written in Python, is built upon NumPy, SciPy and Matplotlib.
 <h4><b>Plotly:-</h4></b>  The plotly is an interactive, open-source plotting library that supports over 40 unique chart types covering a wide range of statistical, financial, geographic, scientific, and 3-dimensional use-cases.
 <h4><b>Seaborn:-</h4></b>  Seaborn is a library that uses Matplotlib underneath to plot graphs. It will be used to visualize random distributions.
 <h4><b>Datetime:-</h4></b>  The Datetime module supplies classes for manipulating dates and times. While date and time arithmetic is supported, the focus of the implementation is on efficient attribute extraction for output formatting and manipulation.
 <h4><b>Statsmodels:-</h4></b>  Statsmodels is a Python module that provides classes and functions for the estimation of many different statistical models, as well as for conducting statistical tests, and statistical data exploration.

<h3><b>Plotting various graphs for different parameters.</b></h3>

<h3><b>Finding the key facts and relationships between various parameters.</b></h3>

<h3><b>Observations according to the outputs of the graph visualizations.</b></h3>

## <b>Conclusion</b>
Comparison of RMSE values for Test Data as lower the RMSE better the model performance:

LinearRegressor RMSE: 7.487
Ridge Regression RMSE: 7.485
Lasso Regression RMSE: 7.741
Elastic Net Regression RMSE: 8.788
DecisionTreeRegressor RMSE: 5.233
RandomForestRegressor RMSE: 4.027
XGBoostRegressor RMSE: 4.824
GradientBoostingRegressor RMSE: 4.824

• XGBoost Regressor and Gradient Boost Regressor give the highest R2 score of 98% and 96% respectively for the Train dataset and 91% for both regressor's Test dataset.So, We can deploy these models.
• The Temperature, Hour & Functioning Day are the most important features that positively drive the total rented bikes count.
• In conclusion, the demand prediction for the given Seoul bike sharing dataset can be accurately predicted using XGBoost Regressor and Gradient Boost Regressor.

