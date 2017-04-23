# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A: *First,find all instances of naked twins;Then,in every box of every common peers of every couple twins delete the two string of corresponding twins*
*Naked twins have the following feature:
- consider only two box.
- there are same two digits in every box of the two box.
steps to sovle the naked twins:
- find all instances of naked twins based on the features
- since in every unit one digit can't appear twice, so the digits of the naked twins can't appear in other box of the common peers of the two box of the naked twins,and then we can delete the two digits of the naked twins in every box of the common peers of the two box of the naked twins.
*

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: *Different from regular sudoku problem,the diagonal sudoku prolem gets new constraint propagation(a type of inference):there will be no same digit appearing in the two diagonal besides rows,columns and squares.Using constraint propagation will reduce the search space obviously.So I add the two diagonal into the constraint propagation of regular sudoku.Then I solve the diagonal sudoku problem same as regular sudoku*

### Install

This project requires **Python 3**.

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project.
Please try using the environment we provided in the Anaconda lesson of the Nanodegree.

##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

### Code

* `solutions.py` - You'll fill this in as part of your solution.
* `solution_test.py` - Do not modify this. You can test your solution by running `python solution_test.py`.
* `PySudoku.py` - Do not modify this. This is code for visualizing your solution.
* `visualize.py` - Do not modify this. This is code for visualizing your solution.

### Visualizing

To visualize your solution, please only assign values to the values_dict using the ```assign_values``` function provided in solution.py

### Data

The data consists of a text file of diagonal sudokus for you to solve.
