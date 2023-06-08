# buenos-aires-house-price-prediction

Predicting the prices of houses based on a number of features given in the dataset. 
I have used various data cleaning and data analysis techniques for this project. The processes used are briefly listed as follows;
1. Defining a `wrangle` functioon to import the csv file, with already cleaned data. 
2. Collecting data from different datasets and importing them in a single dataset.
3. `glob` is used to find patterns in file names and and make a list of the files (datasets) containing Buenos Aires house pricing info.
4. **List comprehension** is used to apply the `wrangle` function to the pathways imported via `glob`.
5. Concatinating the imported datasets into a main dataset, `df`.
6. Dropping the **null** values.
7. Dropping the **Low and High Cardinality categorical features**.
8. Dropping the **Leaky Columns**.
9. Dropping the **Multi Collinearity columns** (collinearity within the variables and not the target variable)

 **Building a Model**
 1. Used a baseline model (with `y_mean` as the baseline prediction)  to test the performance.
 2. Made a pipeline with `SimpleImputer` , `OneHotEncoder` , and `Ridge` algorithms.
 
