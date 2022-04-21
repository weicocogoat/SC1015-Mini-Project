# SC1015 Data Science Mini-Project - Stocks

## About
In this repository, we will be attempting to find the top factors that affect the performance of a stock, so as to develop a safe stock investing strategy to ensure positive rates of return for investors while minimizing losses. We will be mainly focusing on the [US Stock Market data](https://www.kaggle.com/datasets/cnic92/200-financial-indicators-of-us-stocks-20142018) taken from kaggle

## Models used
- Decision Tree
- Random Forest
- GridSeach Cross-Validation
- Time series

## Folder descriptions

### 1. [Data Preparation](https://github.com/weicocogoat/SC1015-Mini-Project/tree/master/1%20data%20preparation)

    Contains:- 
    - 2 CSV files (before and after cleaning)
    - Python Notebook for data cleaning
    
    In this folder, we are doing basic data preparation before moving on to analysis. 
    This includes filling Nan values in the dataset and removing outliers.
   
### 2. [Exploratory Data Analysis](https://github.com/weicocogoat/SC1015-Mini-Project/tree/master/2%20EDA)

    Contains:-
    - 2 CSV files (before and after EDA)
    - Python Notebook for EDA
    
    In this folder, we will be exploring the dataset. We looked into the importance of columns "Price Var" and "Class". 
    Realising that there are too many factors to work with, we cut down that number down into a workble size.
    Utilizing correlation heatmaps, boxplots and violin plots, we explored the factors and found the most relavant factors
    to be used in our machine learning model.
  
### 3. [Model Building](https://github.com/weicocogoat/SC1015-Mini-Project/tree/master/3%20ML)

    Contains:-
    - Dataset after EDA in CSV format
    - Python Notebook for Building the Model
    - Model in sav format
    
    In this folder, we are utilizing decision tree, random forest and GridSearch to create a machine learning model which
    can help us predict the "Class" of a stock. This would let us know whether a stock is profitable or not.
    In the notebook, we explore the various models to look at how do we improve our classification accuracy.
    
### 4. [Strategy for investing based on our model](https://github.com/weicocogoat/SC1015-Mini-Project/tree/master/4%20strategy)
    
    Contains:-
    - Model in sav format
    - 4 CSV files containing datasets from different years to test our model on
    - Python Notebook for looking into what strategy should we consider to maximize profit while minimizing losses.
    
    In this folder, we will be using our model to predict the "Class" variables of the various stocks in different years.
    We then proceeded to propose 3 different strategies for investing based on our model, ran a simulation and plotted 
    the results in a time series graph. After some analysis of the time series graph, we obtained the best strategy for 
    an investor to maximize profit while minimizing losses.
    
## Contributors
- Harvey - Presenter + Editor
- Kasidis - Data Preparation + EDA + Strategy
- Wei Yang - Model building + Slides

## References
- <https://www.kaggle.com/datasets/cnic92/200-financial-indicators-of-us-stocks-20142018>
- <https://slidesgo.com/theme/difference-between-cryptocurrency-and-stocks#search-stocks&position-2&results-6>
- <https://storyset.com/>
- <https://investoracademy.org/3-reasons-why-you-should-care-about-stock-market/>
- <https://www.shmoop.com/finance/investing/why-should-i-care-stocks.html>
- <https://www.investopedia.com/terms/s/shortselling.asp>
- <https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html>
- <https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html>
- <https://www.youtube.com/watch?v=HdlDYng8g9s&t=490s>
