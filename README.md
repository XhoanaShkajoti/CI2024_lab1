# CI2024_lab1
CI2024_lab1
Given a family of sets, find the subfamily of minimum cost that covers all elements in the universe.\
Solve efficiently these instances customizing a technique discussed in class

| Instance | Universe size | Num sets | Density |
|----------|---------------|----------|---------|
| 1        | 100           | 10       | 0.2     |
| 2        | 1,000         | 100      | 0.2     |
| 3        | 10,000        | 1,000    | 0.2     |
| 4        | 100,000       | 10,000   | 0.1     |
| 5        | 100,000       | 10,000   | 0.2     |
| 6        | 100,000       | 10,000   | 0.3     |

# Description 
The algorithm based on **hill climbing** gives priority to improving the current solution, accepts worse solutions (**simulated annealing**) as temperature increases with multiple tweaks.
# Run
To run in a virtual environment follow the istructions [here](https://github.com/squillero/computational-intelligence/tree/master/2024-25/contrib/poetry_installation_guide) (skipping the creation of .toml and .ipynb files)
# Performance
The following table shows some sample performance; all solutions are valid. **The number of steps has been fixed to 5000 in every instance.** \
The solution index represents the number of steps taken to find the best solution. \
The solution's cost is negative, with values closer to zero being better.
| Instance | Solution index | Cost of solution 
|----------|---------------|----------|
| 1        | 477           | -265       |
| 2        | 3979         | -6691      |
| 3        | 5000        | -375010   | 
| 4        | 4999       | -92091461   | 
| 5        | 992      | -228919157  | 
| 6        | 998       | -358552296   | 

instance 5 and 6 were perfomed on 1000 steps while the rest on 5000 steps.
# Contributors
Some techniques implemented in my proposal were discussed and developed jointly with my colleagues [@FerraiuoloP](https://github.com/FerraiuoloP/) (on different occasions)\
We started from the same template, then we discussed how simulated annealing would work in our scenario and we sort of implemented it together (although our versions differ).

