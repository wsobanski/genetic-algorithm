# About

Simple implementation of genetic algorithm for solving n Queens problem.

# Evolution process

This project implements genetic algorithm for solving n Queens problem.
Code generates random population od declared size where every invidual is represented by list containg row position on the board.
One individal represents one setting of queens on the board. 
For example positions of queens on the picture below are represented as: [5, 10, 8, 1, 3, 9, 7, 2, 0, 6]

![solution](https://user-images.githubusercontent.com/94312553/232295940-0c19d59c-bf1b-467c-9cd9-68218fea93d2.png)

Initial population undergoes multiple evolution processes that generates new, stronger population.
Every epoch population is corssed-over, creating x new individuals, where x is size of the initial population. Crossovers are created
by randomly selecting parents based on their scores - the higher the score, the greater the probability of being selected as a parent
for crossover. After that, population of size 2x is randomly mutated with declared chance of being mutated. Then scores are calculated
again to select x best performing individuals. This process is repeated by declared number of iterations or unitl the solution is found.

# Training visualization

This graph represents training process for solution shown above. 
![training](https://user-images.githubusercontent.com/94312553/232299070-09099780-76dc-4b23-9843-1d8f7a9bcdca.png)

# Benchmark

This graph shows comparision in number of iterations needed to find a solution using genetiv algorithm vs randomly selecting population.
This benchmark has been created for population of size 10 and board size of 10.
For both, random search and genetic algorithm there were 35 attempts undertaken.

![benchmark](https://user-images.githubusercontent.com/94312553/232299258-5afdeda1-b607-44be-9312-d4a0a1d4c291.png)
