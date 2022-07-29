# **Iris Flower Classification using KNN**
## Project Description
This project uses K-Nearest-Neigbor Classification to classify 75 flowers from `test.csv` into 3 types of Iris flowers, either **versicolor**, **virginica**, or **setosa** based on training data from `train-2.csv`. KNN is a simple algorithm that stores all available cases and classifies new cases based on a similariy measure. In this case we use the Eucledian Distance Function to calculate similarity.
 
 ![ED](https://camo.githubusercontent.com/c6e4b603e3d6f384292b54dedb384dfab1783b2bd9ec4aaec47a160d3c1647c5/687474703a2f2f7777772e7361656473617961642e636f6d2f696d616765732f4b4e4e5f73696d696c61726974792e706e67)

## Operating Environment
Python 3.9.6 64-bit // Jupyter Notebooks

## Implementation and Execution
1. Open up your virtual environment, Jupyter Notebook and select a Python interpreter. 
2. Change working directory to the folder where `iris_flower_knn.ipynb`, `test.csv` and `train-2.csv` are stored.
3. The project requires **Pandas**, **Numpy** and **CSV** libraries, make sure to have those installed.
4. Run all lines. 

## Code Breakdown

* The first 3 lines of code import the necessary libraries. **Numpy**, **Pandas** and **CSV**. 
* Next, the code takes both the test and training data as input.
* We define the 2 functions below, which help us find the Eucledian Distance as similarity measure.
```
ALL_Distance(iris_train, iris_test):
Euclidean_Distance(iris_train, row):
```
* The code drops unnecessary collumns from the test and training data.
* It then runs the two defined functions above on our test and training data.
* We then define `k_list` for values `1,3,5,7,9` as required in the project description.
* The next block of code uses the unweighted vote of the K nearest examples and breaks the tie by choosing the class with the lowest total distance.
* The code then iterates through each row and returns the desired output.



