### EX NO: 01
### DATE : 04-04-2022
# <p align="center"> RANDOM CLASSIFICATION</p>
## AIM:
To write a python program to perform random classification.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Google Colab /Jupiter Notebook

## Concept: 
Random forest is a supervised learning algorithm which is used for both classification as well as regression.Regression is a technique for investigating the relationship between independent variables or features and a dependent variable or outcome. It is mainly used for classification problems. It creates decision trees on data samples and then gets the prediction from each of them. Finally, it selects the best solution by means of voting. Voting is an ensemble method which is better than a single decision tree because it reduces the over-fitting by averaging the result.An overfitting model fits the training data too well, but it fails to do this on the new data.

## Libraries Used in the program.

## NUMPY 
NumPy is a library for the Python programming language, adding support for large, multidimensional arrays and matrices, along with a large collection of high-level mathematical functions to operate on these arrays. 

## SKLEARN  
Scikit-learn is a free software machine learning library for the Python programming language. It features various classification, regression and clustering algorithms including support-vector machines. 

## MATPLOTLIB  
Matplotlib is a plotting library for the Python programming language and its numerical mathematics extension NumPy. It provides an object-oriented API for embedding plots into applications using generalpurpose GUI toolkits like Tkinter, wxPython, Qt, or GTK. 

## Algorithm 
1.	Start the program. 
2.	Import libraries required as per requirement. 
3.	Define dataset use the make_blobs() function to generate a synthetic multi -class classification dataset. 
4.	summarize dataset shape.
5.	summarize observations by class label.
6.	summarize first few examples. 
7.	plot the dataset and color the by class label.
8.	stop the program. 
 
## Program Code: 

/*
Program to implement random classification.

Developed by   :U.VIVEK KRISHNA

RegisterNumber :212219040180
*/

import matplotlib.pyplot as plt 

from sklearn import datasets 

X, y = datasets.make_blobs(n_samples=150,n_features=2, centers=2,cluster_std=1.05, random_state=2)  

fig = plt.figure(figsize=(10,8))

plt.plot(X[:, 0][y == 0], X[:, 1][y == 0], 'r^') 

plt.plot(X[:, 0][y == 1], X[:, 1][y == 1], 'bs')

plt.xlabel("feature 1")

plt.ylabel("feature 2") 

plt.title('Random Classification Data with 2 classes') 

## Output:
![image](https://user-images.githubusercontent.com/63917883/166445820-99314a80-dce1-41aa-9b8a-7d2bec9bad53.png)

## Result:
Thus the random classifier was successfully implemented using python programming.

