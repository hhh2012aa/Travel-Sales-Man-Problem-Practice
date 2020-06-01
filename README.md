# Travel-Sales-Man-Problem-Practice

Two Efficient way to solve Travel Sales Man Problem (TSP) on Python, we only have to Input distance maxtrix to receive optimum.

## 1. [Tsp module] (https://pypi.org/project/tsp/) on PyPI 

  #### step (1) `$ pip install pipy`
  
  #### step (2) open your Python IDE and Paste:
  ```mat = {your_distance_matrix}
  r = range(len(mat))
  dist = {(i, j): mat[i][j] for i in r for j in r}
  print(tsp.tsp(r, dist))
  ```
  
  The total distance and tour will be shown like this `(4, [0, 1, 3, 2])`

  
#＃ 2. Solve by Gurobipy
