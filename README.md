# An implementation of a GA to solve the Asymmetric Traveling Salesman Problem
In this project, an implementation of GA is presented and implemented in Python. In addition to the model, this repository contains a set of test instances for evaluation.

## Dependencies
- Numpy
- Pandas
- Matplotlib

## Instalation and execution
- Put the *Algorithm.ipynb* file (alternatively, the *Algorithm.py* file) and the *.txt* document containing the distance matrix of the problem in the same folder. The *.txt* document must be in a standard format (see one of the test instances provided in the **TestInstances** folder).
- Open the *Algorithm.ipynb* file using Jupyter Notebook (or the *Algorithm.py* with the Python development environment that you prefer)
- Modify the path/name of the *.txt* file that contains the instance to be evaluated, and the algorithm parameters according to your requirements
- Run.

## An example
The documentation provided includes a set of test instances (**TestInstances** folder) for evaluating the algorithm. As an example, we consider applying the algorithm to one of the instances provided in the set of test instances (Instance 4). We consider two versions of the model, applying different parameters for the same instance.
- For Version 1, we consider:
  - X
- For Version 2, we consider:
  - X

When applying Version 1 to the test instance, Figure 2 shows the value of the Fitness function (i.e. the final distance of the obtained circuit), with respect to each of the generations. In the illustration it can be seen how the value of the function converges, which reflects the tendency of the algorithm to refine the value of the solution following an elitist criteria.

On the other hand, Figure 3 shows the value of the Fitness function obtained for each generation when applying Version 2 of the algorithm. The illustration shows the significant incidence of the Probability of Mutation parameter in the quality of the solutions found. That is, the proposed algorithm is highly sensitive to this parameter, and increasing its value can considerably affect the value of the solutions found, so it would be advisable to keep it at values of the same order of magnitude as that proposed in Version 1. This could reduce exploratory potential or diversification of solutions from the proposed algorithm, but it is left to the discretion of the user according to their interest.
