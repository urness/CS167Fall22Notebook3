# Notebook #3: Cross Validation with kNN and Life Expectancy

## The Data: 
For this notebook, you're going to work with a k-NN function you made for predicting life expectancy for developing countries from Notebook 2. This time, however, use only the data with `'Status' == 'Developing'` and use the features `['Life expectancy', 'Polio', 'Diphtheria', 'Hepatitis B']` with "Life expectancy" being the target feature. (Presumably, this could be a step in investigating the effectiveness of vaccine data (for Polio, Diphtheria, and Hepatitis B) in predicting life expectancy in developing countries.)

The goal of this assignment is to use **cross-validation** in the kNN model to determine the optimal use of k in the algorithm. This will required the use of independent training and test subsets of the data. 

For an example of this using the Iris dataset, see the notes from Lecture 7 and Lecture 8, ([or this GitHub repository](https://github.com/urness/CS167Fall22Code))

## What you need to do: 

- Don't forget that you are doing regression-- pay attention to what you need to change to make this do regression rather than classification.
- Make sure to implement an appropriate regression metric - you should use **mean squared error** for this assignment. 
- Make sure your variables and functions all have reasonable names. I will deduct points if variables/functions are named things such as "iris" or "classification" (as this is a regression problem).

1. Implement mean squared error (mse) algorithm  
    `def mse(actual,predicted):`
    
2.  Implement the testing and training data. Use the approximately the first 500 rows in the shuffled set as testing data. Feel free to use fewer examples in your testing set -- particularly if it takes a long time to run on your computer (e.g. more than 30 seconds). 
3. Test your model using several different values of k and **graphically show the results**.
4. Run this for several different splits of the data -- varying the number of elements in the testing data and/or different values for the "random_state". 
5. What conclusions can you draw about the best number for k for the k-NN algorithm for this data set? Use a markdown cell to explain your conclusions in a few sentences.

## :white_check_mark: Grading: 
I will update the following rubric with your grade after you have completed the assignment.
### Rubric:
| Exercise #  | Points Awarded (out of 1)  | Notes |
| --------- | ------------------- | --------- |
| 1: mse                   |        |    |
| 2: test data             |        |    | 
| 3: graph results         |        |    |
| 4: splits of data        |        |    | 
| 5: conclusions           |        |    |
| <b>Total                 |    /5  | </b>|
