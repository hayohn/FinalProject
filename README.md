# Analyzing Demographic Indicators Using Machine Learning

## Table of Contents
1. [Objective](#objective)
2. [Dataset](#dataset)
3. [Methodology](#methodology)
    - [Dataset Clean-up](#dataset-clean-up)
    - [Data Collection, Preprocessing and Exploratory Data Analysis (EDA)](#data-collection-preprocessing-and-exploratory-data-analysis-eda)
    - [Clustering Analysis - Unsupervised Machine Learning](#clustering-analysis---unsupervised-machine-learning)
    - [Models Regression - Supervised Machine Learning](#models-regression---supervised-machine-learning)
    - [Presentation and Reporting](#presentation-and-reporting)
4. [Technologies Used](#technologies-used)
5. [Timeline](#timeline)
6. [Word Analysis](#word-analysis)

## Objective
The goal of this project is to explore and analyze demographic data by country for the year 2020, using machine learning techniques to uncover insights and compare key indicators across countries. We aim to answer the following questions:
- What are the relationships between fertility rate, life expectancy, median age, population growth, sex ratio, suicide rate, and urbanization rate across countries in 2020?
- Can we identify distinct clusters or groups of countries that emerge based on these indicators in 2020?
- How do the selected countries compare in terms of these indicators in 2020?

## Dataset
We will be using a dataset containing information on fertility rate, life expectancy, median age, population growth, sex ratio, suicide rate, and urbanization rate for various countries in the year 2020. The dataset has 297 records and includes country names and numerical values for each indicator. The source of the dataset is: [World Data by Country 2020](https://www.kaggle.com/datasets/daniboy370/world-data-by-country-2020).

## Methodology
### Dataset Clean-up
After collecting the dataset, we cleaned up using the Pandas library by merging the CSV files, dropping the missing/zero values and duplicates, and re-ordered the columns.
### Data Collection, Preprocessing and Exploratory Data Analysis (EDA)
We performed several data preprocessing steps, including:
- Dropping missing values
- Removing duplicates
- Encoding categorical variables ('Country' and 'ISO-code')
- Scaling numerical variables ('Fertility', 'Life expectancy', 'Median age', 'Population growth', 'Sex-ratio', 'Suicide rate', 'Urbanization rate')
- Train-Test Split: The code splits the dataset into training and test sets, with 'Life expectancy' set as the target variable and the remaining variables as features.
- Descriptive statistics of the dataset are printed, providing summary statistics for each numerical column. The correlation matrix is calculated and visualized using a heatmap, showing the correlations between variables. A scatter plot matrix and a pairplot matrix are also created to visualize the pairwise relationships between variables. Distribution plots (histograms and box plots) are generated for each variable.
- 
### Clustering Analysis - Unsupervised Machine Learning
Apply unsupervised learning techniques such as K-means clustering to identify groups of countries with similar demographic profiles in 2020.
- Evaluate the clustering results using appropriate metrics like silhouette score.
- Visualize the clusters using techniques like Principal Component Analysis (PCA) and interactive scatter plots.
- 
### Models Regression - Supervised Machine Learning
The machine learning models were evaluated using various performance metrics, including R-squared, Mean Absolute Error (MAE), and Mean Squared Error (MSE). The results show that the Random Forest Regressor and Decision Tree Regressor perform exceptionally well in predicting life expectancy based on the given demographic indicators.

### Presentation and Reporting
Prepare a comprehensive report detailing the project's objectives, methodology, results, and conclusions.
- Create a presentation to showcase the project's findings using a combination of slides, visualizations, and live demonstrations.

## Technologies Used
- Python
- Pandas
- Matplotlib
- Plotly
- NumPy
- Seaborn
- Math
- Scikit-learn

## Timeline
- Week 1: Data collection, preprocessing, and exploratory data analysis
- Week 1: Machine learning model building, training, and evaluation
- Week 2: Clustering analysis and time series analysis
- Week 2: Results interpretation, visualization, and reporting

## Word Analysis
Perform word analysis on the dataset to extract insights and visualize them.
