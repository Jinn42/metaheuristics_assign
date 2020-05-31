# metaheuristics_optim
## Discrete Optimization:
### The approach:

Let’s start with a few definitions, rephrased in the context of the TSP:

Gene: a city (represented as (x, y) coordinates)
Individual (aka “chromosome”): a single route satisfying the conditions above
Population: a collection of possible routes (i.e., collection of individuals)
Crossover: this crossover uses 3 parents, A and B provide the "genes", C is used to determine the shape	
Fitness: a function that tells us how good each route is (in our case, how short the distance is)
Mutation: a way to introduce variation in our population by randomly swapping two cities in a route
Preselection: To determine a better initial population rather than producing an initial population randomly. The realization is achieved by using resolve function to link points within certain distances (controlled by the parameter epsilon)
Resolve function: This function resolves (more or less) the crossings in a path by "twisting" loops (imagine you want to turn "8" to “0”. For every 50 generations we applied resolve functions (The more frequently the resolve function is applied, the longer the run time)

### Parameters:
max_generation=300
epsilon= 100 / 150 (different epsilon results in different result)

### Result of Fitness:
![image](https://github.com/Jinn42/metaheuristics_optim/blob/master/images/city_38_194_result.png)

### For 38 cities:
![image](https://github.com/Jinn42/metaheuristics_optim/blob/master/images/city_38_map.png)
