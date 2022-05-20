# RANDOM CLASSIFICATION

## Aim:
To write a python program to perform random classification.


## Equipments Required:
Hardware – PCs

Anaconda – Python 3.7 Installation / Google Colab /Jupiter Notebook



## Related Theoritical Concept:
A Random Forest is a meta estimator that fits a number of decision tree classifiers on various sub-samples of the dataset and uses averaging to improve the predictive accuracy and control over-fitting.Random forest classifier creates a set of decision trees from randomly selected subset of training set. It then aggregates the votes from different decision trees to decide the final class of the test object.


## Algorithm
1.In Random forest n number of random records are taken from the data set having k number of records.

2.Individual decision trees are constructed for each sample.

3.Each decision tree will generate an output.

4.Final output is considered based on Majority Voting or Averaging for Classification and regression respectively.


## Program
```
/*
Program to implement random classification.
Developed by   : SANJU S
RegisterNumber :  212219040137
*/
import matplotlib.pyplot as plt
from sklearn import datasets
X,y = datasets.make_blobs(n_samples=100,n_features=2,centers=2,cluster_std=1.05,random_state=2)
fig=plt.figure(figsize=(10,8))
plt.plot(X[:,0][y==0], X[:,1][y==0],'pc')
plt.plot(X[:,0][y==1], X[:,1][y==1],'bo')
plt.xlabel("Feature 1")
plt.ylabel("FeaTure 2")
plt.title("Random Classification Data with 2 classes")
```


## Output
![download](https://user-images.githubusercontent.com/94214195/169483695-50d8d658-cf3e-493a-aae7-ecec5e925c83.png)



## Result:
Thus the random classifier was successfully implemented using python programming.
