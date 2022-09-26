# Notebook #3: Cross Validation with kNN and Wine Ratings

## The Data: 
For this notebook, you're going to work with a k-NN function for predicting the 'quality' of white wine :wine. The [white wine quality data set] (https://archive.ics.uci.edu/ml/datasets/wine+quality) has a 'quality' colum (a range from 0 to 10) and will serve the target feature we are trying to predict. The data has the following predictor columns:

1 - fixed acidity
2 - volatile acidity
3 - citric acid
4 - residual sugar
5 - chlorides
6 - free sulfur dioxide
7 - total sulfur dioxide
8 - density
9 - pH
10 - sulphates
11 - alcohol

You do not need to know what any of the above means; it is sufficient to know that they are all numeric values that measure some aspect of a wine. The dataset consists of 1599 training examples. The goal of this assignment is to use **cross-validation** in the kNN model to determine the optimal use of k in the algorithm for predicting wine quality. This will required the use of independent training and test subsets of the data. 

For an example of this using the Iris dataset or the Penguin dataset to help solve similar problems, see the notes from Lecture 7 and Lecture 8, ([or this GitHub repository](https://github.com/urness/CS167Fall22Code))

## What you need to do: 

- Don't forget that you are doing regression -- pay attention that the implementation to kNN uses the average 'quality' of the top k training examples.
- Make sure to implement an appropriate regression metric - you should use **mean squared error** for this assignment. 
- Make sure your variables and functions **and graph labels/titles** all have reasonable names. I will deduct points if variables/functions are named things such as "iris" or "classification" (as this is a regression problem).

1. Implement mean squared error (mse) algorithm  
    `def mse(actual,predicted):`
    
2.  Implement the testing and training data. Use the approximately the first 320 rows in the shuffled set as testing data. Feel free to use fewer examples in your testing set -- particularly if it takes a long time to run on your computer (e.g. more than 30 seconds). 
3. Use the code provided to normalize the data. Test your model using several different values of k and **graphically show the results** using your implementation of mse.
4. Repeat the experiment and **graphically show the results** using r^2.
5. Describe your findings. What conclusions can you draw about the best number for k for the k-NN algorithm for this data set? Use a markdown cell to explain your conclusions.

## :white_check_mark: Grading: 
I will update the following rubric with your grade after you have completed the assignment.
### Rubric:
| Exercise #  | Points Awarded (out of 1)  | Notes |
| --------- | ------------------- | --------- |
| 1: mse                   |        |    |
| 2: test data             |        |    | 
| 3: graph results mse        |        |    |
| 4: graph results r^2        |        |    | 
| 5: conclusions           |        |    |
| <b>Total                 |    /5  | </b>|
