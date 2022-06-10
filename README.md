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
Also, a One Hot coding was performed to be able to work with numerical data.

## Machine learning models
Three machine learning algorithms were tested for this database, which were **KNN, Decision Trees** and **Random Forest**.

## Results for KNN
For the implementation of this algorithm, different values of K nearest neighbors are tested, and both the error and the accuracy obtained are plotted.

![error_gr](https://user-images.githubusercontent.com/44073142/172978326-14e5b3cc-4118-4283-a3f5-c3b75387ebdf.png)
![accuracy_gr](https://user-images.githubusercontent.com/44073142/172978316-6015137e-f551-4468-93d7-5b8af5199da7.png)

Observing this graphs, it was determined that the optimal value for K nearest neighbors is 12.
The classification report and the resulting confusion matrix are shown below. 

![reporte_knn](https://user-images.githubusercontent.com/44073142/172980061-aedcc439-b19a-43f7-b71b-9e48578ec70f.png)
![matriz_knn](https://user-images.githubusercontent.com/44073142/172980027-6793a20f-2f55-443d-b925-bf2c729abf68.png)
