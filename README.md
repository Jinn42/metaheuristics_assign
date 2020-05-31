# metaheuristics_optim
## Discrete Optimization:
### The approach:

Let’s start with a few definitions, rephrased in the context of the TSP:

**Gene**: a city (represented as (x, y) coordinates)  
**Individual** (aka “chromosome”): a single route satisfying the conditions above  
**Population**: a collection of possible routes (i.e., collection of individuals)  
**Crossover**: this crossover uses 3 parents, A and B provide the "genes", C is used to determine the shape  	
**Fitness**: a function that tells us how good each route is (in our case, how short the distance is)  
**Mutation**: a way to introduce variation in our population by randomly swapping two cities in a route  
**Preselection**: To determine a better initial population rather than producing an initial population randomly. The realization is achieved by using resolve function to link points within certain distances (controlled by the parameter epsilon)  
**Resolve function**: This function resolves (more or less) the crossings in a path by "twisting" loops (imagine you want to turn "8" to “0”. For every 50 generations we applied resolve functions (The more frequently the resolve function is applied, the longer the run time)

### Parameters:
max_generation=300;
epsilon= 100 / 150 (different epsilon results in different result)

### Result of Fitness:
<img width="500" height="100" src="https://github.com/Jinn42/metaheuristics_optim/blob/master/images/city_38_194_result.png" />


### For 38 cities:
|map|fitness|
|:---|:---|
|<img width="250" height="250" src="https://github.com/Jinn42/metaheuristics_optim/blob/master/images/city_38_map.png" />|<img width="250" height="250" src="https://github.com/Jinn42/metaheuristics_optim/blob/master/images/city_38_fitness(1).png" />|


### For 194 cities:
|map|fitness|
|:---|:---|
|<img width="250" height="250" src="https://github.com/Jinn42/metaheuristics_optim/blob/master/images/city_194_map.png" />|<img width="250" height="250" src="https://github.com/Jinn42/metaheuristics_optim/blob/master/images/city_194_fitness.png" />|

## Continuous Optimization:
### For the 6 functions, all algorithms are from spicy package, the selection of algorithm for each is based on the result of fitness

### Parameters:
Search Space:  [-100, 100];
'maxiter': 100;
'ftol': 1e-05


### Result of Fitness:
 <img width="900" height="100" src="https://github.com/Jinn42/metaheuristics_optim/blob/master/images/result.png" />

### F1:
|D=50|D=500|
|:---|:---|
|<img width="300" height="600" src="https://github.com/Jinn42/metaheuristics_optim/blob/master/images/F1_D50.png" />|<img width="300" height="600" src="https://github.com/Jinn42/metaheuristics_optim/blob/master/images/F1_D500.png" />|

### F2:
|D=50|D=500|
|:---|:---|
|<img width="300" height="600" src="https://github.com/Jinn42/metaheuristics_optim/blob/master/images/F2_D50.png" />|<img width="300" height="600" src="https://github.com/Jinn42/metaheuristics_optim/blob/master/images/F2_D500.png" />|

### F3:
|D=50|D=500|
|:---|:---|
|<img width="300" height="600" src="https://github.com/Jinn42/metaheuristics_optim/blob/master/images/F3_D50.png" />|<img width="300" height="600" src="https://github.com/Jinn42/metaheuristics_optim/blob/master/images/F3_D500.png" />|

### F4:
|D=50|D=500|
|:---|:---|
|<img width="300" height="600" src="https://github.com/Jinn42/metaheuristics_optim/blob/master/images/F4_D50.png" />|<img width="300" height="600" src="https://github.com/Jinn42/metaheuristics_optim/blob/master/images/F4_D500.png" />|

### F5:
|D=50|D=500|
|:---|:---|
|<img width="300" height="600" src="https://github.com/Jinn42/metaheuristics_optim/blob/master/images/F5_D50.png" />|<img width="300" height="600" src="https://github.com/Jinn42/metaheuristics_optim/blob/master/images/F5_D500.png" />|

### F6:
|D=50|D=500|
|:---|:---|
|<img width="300" height="600" src="https://github.com/Jinn42/metaheuristics_optim/blob/master/images/F6_D50.png" />|<img width="300" height="600" src="https://github.com/Jinn42/metaheuristics_optim/blob/master/images/F6_D500.png" />|
