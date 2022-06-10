# Mushrooms dataset project

## Summary
In this project, *Machine Learning* knowledge is applied using the **Mushrooms database** for the classification of edible or poisonous mushrooms. This database is found [here](https://www.kaggle.com/datasets/uciml/mushroom-classification). 

## Database Description
This database contains 23 attributes in order to describe whether mushrooms are edible or not, as well as 8124 instances.

![base](https://user-images.githubusercontent.com/44073142/172974520-47b496ec-88e1-41ff-8419-387cdcc5db17.png)

The mushrooms classification consists of 2 classes:
- e, edible
- p, poisonous

## Data processing
The data analysis was performed in order to search for missing values or attributes that do not contribute to the database. Once the missing values were found in the database, these values were imputed, using the technique of imputation by mode. After this, two techniques (Cramer's V and Theil's U) were used to find the association of categorical variables, and thus be able to select the attributes to implement the machine learning models. 
