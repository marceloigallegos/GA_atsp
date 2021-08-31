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

The output of the model corresponds to:
- The distance of a random circuit, considered as an initial solution.
- The distance of the circuit obtained as a solution.
- The description of the circuit obtained, in the structure of a sequentially ordered vector. Thus, the first node of this vector will be the start node of the circuit (and the last one will be the end node).
- A graphic representation of the solutions obtained by the algorithm, according to the number of generations assigned as a parameter.

## An example
The documentation provided includes a set of test instances (**TestInstances** folder) for evaluating the algorithm. As an example, we consider applying the algorithm to one of the instances provided in the set of test instances (Instance 4). We consider two versions of the model, applying different values for the Mutation Rate Parameter for the same instance.
- For Version 1, we consider:
  - A population size (*n_Poblacion*) of 200 individuals.
  - A elite sample size (*n_Elite*) of 40 individuals.
  - **A mutation rate (*p_Mutacion*) of 0.1%**.
  - A total of 800 generations (*generaciones*).

- For Version 2, we consider:
  - A population size (*n_Poblacion*) of 200 individuals.
  - A elite sample size (*n_Elite*) of 40 individuals.
  - **A mutation rate (*p_Mutacion*) of 1%**.
  - A total of 800 generations (*generaciones*).

![alt text](https://github.com/marceloigallegos/GA_atsp/blob/main/mdImages/Fig1.png)

When applying Version 1 to the test instance, figure above shows the value of the Fitness function (i.e. the final distance of the obtained circuit), with respect to each of the generations. In the illustration it can be seen how the value of the function converges, which reflects the tendency of the algorithm to refine the value of the solution following an elitist criteria.

![alt text](https://github.com/marceloigallegos/GA_atsp/blob/main/mdImages/Fig2.png)

On the other hand, figure above shows the value of the Fitness function obtained for each generation when applying Version 2 of the algorithm. The illustration shows the significant incidence of the Probability of Mutation parameter in the quality of the solutions found. That is, the proposed algorithm is highly sensitive to this parameter, so it would be advisable to keep it at values of the same order of magnitude as that proposed in Version 1 if the priority of your work is to find good quality solutions. On the contrary, if you are interested in expanding the exploration and diversification potential of the method, this parameter should be where you focus your attention.
