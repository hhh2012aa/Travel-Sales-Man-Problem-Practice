# Solve Travel Sales Man Problem

Two Efficient way to solve Travel Sales Man Problem (TSP) on Python, we only have to Input distance maxtrix to receive optimum.

## 1. [Tsp module](https://pypi.org/project/tsp/) on PyPI 

  #### Step (1): `$ pip install pipy`
  
  #### Step (2): open your Python IDE and Paste:
  ```mat = {your_distance_matrix}
  r = range(len(mat))
  dist = {(i, j): mat[i][j] for i in r for j in r}
  print(tsp.tsp(r, dist))
  ```
  
  The total distance and tour will be shown like this `(4, [0, 1, 3, 2])`

  
## 2. Solve by [Gurobipy](https://www.gurobi.com/documentation/9.0/quickstart_mac/py_python_interface.html)

  #### Step (1): Follow the step on [Gurobi official Site](hhttps://www.gurobi.com/documentation/9.0/quickstart_mac/py_python_interface.html) to install Gurobi Python module
  
  #### Step (2): Follow the TSP modeling tutoral from [Gurobi official Site](https://gurobi.github.io/modeling-examples/traveling_salesman/tsp.html) to build your formulation and find the optimun.

## 3. Or you can implement other Heuristics/MetaHeuristics 
[Here](Solution.py) is a simple example that I add the randness into common Greedy method and keep itering to find the better solution.
