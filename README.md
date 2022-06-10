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

## Testing
### KNN
For the implementation of this algorithm, different values of K nearest neighbors are tested, and both the error and the accuracy obtained are plotted.

![error_gr](https://user-images.githubusercontent.com/44073142/172978326-14e5b3cc-4118-4283-a3f5-c3b75387ebdf.png)
![accuracy_gr](https://user-images.githubusercontent.com/44073142/172978316-6015137e-f551-4468-93d7-5b8af5199da7.png)

Observing this graphs, it was determined that the optimal value for K nearest neighbors is 12.
The classification report and the resulting confusion matrix are shown below. 

![matriz_knn](https://user-images.githubusercontent.com/44073142/172980027-6793a20f-2f55-443d-b925-bf2c729abf68.png)
![reporte_knn](https://user-images.githubusercontent.com/44073142/172980061-aedcc439-b19a-43f7-b71b-9e48578ec70f.png)

### Decision tree
The classification report and the resulting confusion matrix are shown below. 
![matriz_arbol](https://user-images.githubusercontent.com/44073142/172980716-e5dc35e2-90d8-4dee-982c-9decc62c9f4e.png)
![reporte_arbol](https://user-images.githubusercontent.com/44073142/172980732-9b3b67f3-6a8d-48bd-949f-a12771cb457e.png)

### Random Forest
The classification report is shown below, as well as the resulting confusion matrix.

![matriz_random](https://user-images.githubusercontent.com/44073142/172982242-f1f18026-53b6-4388-9a24-200a2498e17b.png)
![reporte_random](https://user-images.githubusercontent.com/44073142/172982247-2e07dd37-a057-4dc4-aaae-34f0eb7c1142.png)


## Results
### Cross-validation
The purpose of performing the cross-validation was to know the behavior of the models tested with the Mushrooms database, for different values of k-folds. The following figures show graphs with different metrics for the KNN, Decision Trees and Random Forest models.

