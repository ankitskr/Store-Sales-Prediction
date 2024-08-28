# Rossman store sales prediction

## Project Overview
Rossmann operates over 3,000 drug stores in 7 European countries. Currently, Rossmann store managers are tasked with predicting their daily sales for up to six weeks in advance. Store sales are influenced by many factors, including promotions, competition, school and state holidays, seasonality, and locality. With thousands of individual managers predicting sales based on their unique circumstances, the accuracy of results can be quite varied.
In this machine learning project, we will work on forecasting 6 weeks of daily sales for 1,115 stores located across Germany. Reliable sales forecasts enable store managers to create effective staff schedules that increase productivity and motivation. By helping Rossmann create a robust prediction model, we will help store managers stay focused on what’s most important to them: their customers and their teams! 

## Project Aim
1. Perform Feature Importance Analysis, useful to gain feature insights and perform feature selection.
2. Forecast 6 weeks of daily sales using a suitable ML regression model. 

## Data Description
We have been provided data with the following data fields.
1. **Id** - An Id that represents a (Store, Date) duple within the test set
2. **Store** - A unique Id for each store
3. **Sales** - The turnover for any given day (this is what we are predicting)
4. **Customers** - The number of customers on a given day
5. **Open** - An indicator for whether the store was open: 0 = closed, 1 = open
6. **StateHoliday** - Indicates a state holiday. Normally all stores, with few exceptions, are closed on state holidays. Note that all schools are closed on public holidays and weekends. a = public holiday, b = Easter holiday, c = Christmas, 0 = None
7. **SchoolHoliday** - Indicates if the (Store, Date) was affected by the closure of public schools
8. **StoreType** - Differentiates between 4 different store models: a, b, c, d
9. **Assortment** - Describes an assortment level: a = basic, b = extra, c = extended
10. **CompetitionDistance** - Distance in meters to the nearest competitor store
11. **CompetitionOpenSince(Month/Year)** - Gives the approximate year and month of the time the nearest competitor was opened
12. **Promo** - Indicates whether a store is running a promo on that day
13. **Promo2** - Promo2 is a continuing and consecutive promotion for some stores: 0 = store is not participating, 1 = store is participating
14. **Promo2Since(Year/Week)** - Describes the year and calendar week when the store started participating in Promo2
15. **PromoInterval** - Describes the consecutive intervals Promo2 is started, naming the months the promotion is started anew. E.g. "Feb,May,Aug,Nov" means each round starts in February, May, August, November of any given year for that store

**Data Source** : https://www.kaggle.com/c/rossmann-store-sales/data


## Approach
1. **Exploratory Data Analysis**: Exploratory data analysis is the process of analysing the dataset to understand its characteristics. In this step, we will figure out the following.
- Identifying the number of unique users
- Platforms used by the users the most
- Correlations
- Checking for null / inconsistent values and various other insights are drawn.
2. **Imputation**: This step involves the process of filling the missing values in appropriate ways so that the data is not lost.
3. **Outliers Detection and removal**: Outliers are nothing but points that are abnormally distant from the other points. These kinds of outliers present in the data are detected and eliminated.
4. **Further Exploratory Data Analysis**: Further EDA is performed to understand the data more and find out a few exceptional cases.
5. **Label Encoding and One hot encoding**: Machine learning algorithms for regression can understand the input only in the form of numbers and hence it is highly essential to convert the non - numeric data that we have to numeric data by providing them labels.
6. **Model Building and evaluation** Various regression algorithms are applied on the dataset and the model that suits best for the dataset is selected. The models that we apply for this dataset are
- Linear Regression
- SGD Regression
- Decision Tree Regressor
- Random Forest Regressor
7. **Feature Importance Analysis**: Once we have the right model selected (which in our case is Random forest regressor) it is also essential to understand what are the features that contribute the most or least towards the result. 

## Technologies Used
- **Python**: Major programming language used for the project.
- **Pandas & NumPy**: For data manipulation and numerical calculations.
- **Scikit-learn**: For implementing machine learning algorithms.
- **Jupyter Notebook**: For interactive data analysis and sharing of results.

## Working demonstration
A working demonstration is provided in the notebooks folder.
[notebooks/rossman_sales_prediction.ipynb](https://github.com/ankitskr/Store-Sales-Prediction/blob/master/notebooks/rossman_sales_prediction.ipynb)

## Project Takeaways
1. Understanding the problem statement
2. Data exploration
3. Data Visualization
4. Handling missing values
5. Handling Outliers
6. Exploring exceptional cases
7. Converting categorical to numeric forms
8. Creating heatmaps
9. Feature selection & its importance
10. Model implementation and evaluation
11. Understanding feature importance
