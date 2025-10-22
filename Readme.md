This repository contains two data science projects utilizing NBA player data, the contents of which are the following:
- An analysis of the relation between NBA player statistics and salary.
- A forecast of NBA All Star game and NBA MVP selections, based on player performance.

Furthermore, all csv files used for the project are included in the repository as well.

The following tools and technologies are used:

- Python (`pandas`, `NumPy`, `scikit-learn`, `seaborn`, `plotly`)
- Jupyter Notebook
- Git & GitHub for version control

The data used in both projects was sourced from:
- The GraphQL API https://nbaapi.com/graphql/
- Flat files downloaded from Kaggle

## Brief Description

### 1. NBA All Star and MVP Predictions
The main object of this project was to, based on player statistics and selections for previous seasons, make predictions for participants in the NBA All Star game and the winner of the NBA season MVP.
The predictions where made using different machine learning models.
Results where thoroughly reviewed and visualized using a number of model performance metrics. 
Best performance while predicting the All Star game participants was achieved by a XGBoost classifier, with a ROC-AUC score of ~85%.
For the prediction of the NBA MVP, the best result was delivered by a random forest classifier, with an F1 score of 67%.
The project can thus be divided in three main sections:

- Cleaning and transformation of player statistics data  
- Exploratory data analysis with visualizations
- Training of machine learning models (Logistic Regression, Decision Tree, XGBoost Regression, XGBoost Classifier, Naive Bayes Classifier, Random Forest Classifier)
- Performance review of the above, with visualizations

### 2. NBA Salary Prediction
The content of this project is the exploration of the relation of NBA player statistics and salaries throughout various seasons.
To carry this out, a general player rating statistic was defined in order to condense the player performance into a single metric and relating this to player salaries.
The analysis is supported by various visualizations. 
To better quantifiy the relationship, linear and logarithmic regressions were implemented on player salary and rating. 
Lastly, the regression coefficients accross the seasons were plotted.
The main results of the project is that, on average, the salary of NBA players is steadily increasing through the years. 
However, one can observe that this is mainly due to a disproportionate increase in renumeration for NBA stars. 

**How to run the projects:**

1. Clone the repository:
    
        git clone https://github.com/yourusername/nba-data-science-projects.git
        cd nba-data-science-projects

2. Install dependencies:
   
        pip install -r requirements.txt

3. Open Jupyter Notebook:
    
        jupyter notebook

4. Run each notebook.