# Rossman store sales prediction

## Project Overview
Rossmann operates over 3,000 drug stores in 7 European countries. Currently, Rossmann store managers are tasked with predicting their daily sales for up to six weeks in advance. Store sales are influenced by many factors, including promotions, competition, school and state holidays, seasonality, and locality. With thousands of individual managers predicting sales based on their unique circumstances, the accuracy of results can be quite varied.

In this project, we will work developing machine learning models capable of forecasting  daily sales for 1,115 stores located across Germany. Reliable sales forecasts enable store managers to create effective staff schedules that increase productivity and motivation. By helping Rossmann create a robust prediction model, we will help store managers stay focused on what’s most important to them: their customers and their teams! 

**Data Source** : https://www.kaggle.com/c/rossmann-store-sales/data

## Project Aim
1. Build and evaluate ML regression model for sale forecasting.
2. Perform Feature Importance Analysis to gain insights for feature selection.


## Approach
1. **Exploratory Data Analysis**: Exploratory data analysis is the process of analysing the dataset to understand its characteristics. In this step, we will figure out the following.
- Label Encoding and One hot encoding
- Correlations
- Checking for inconsistent values
- Imputation (filling the missing values)
2. **Model Building and evaluation** Various regression algorithms are applied on the dataset and the model that suits best for the dataset is selected. The models that we apply for this dataset are
- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
3. **Feature Importance Analysis**: Once we have the right model selected (which in our case is Random forest regressor) it is also essential to understand what are the features that contribute the most or least towards the result. 


## Technologies Used
- **Python**: Major programming language used for the project.
- **Pandas & NumPy**: For data manipulation and numerical calculations.
- **Scikit-learn**: For implementing machine learning algorithms.
- **Jupyter Notebook**: For interactive data analysis and sharing of results.


## Working demonstration
A working demonstration is provided in the notebooks folder.
- Cleanup and EDA: [notebooks/rossman_sales_cleanup_and_EDA.ipynb](https://github.com/ankitskr/Store-Sales-Prediction/blob/master/notebooks/rossman_sales_cleanup_and_EDA.ipynb)
- Prediction modelling: [notebooks/rossman_sales_prediction_modelling.ipynb](https://github.com/ankitskr/Store-Sales-Prediction/blob/master/notebooks/rossman_sales_prediction_modelling.ipynb)


