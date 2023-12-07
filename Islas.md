# Conteo De Numero de Islas 

~~~python
import numpy as np
#       1   2   3   4   5   6   7   8   9  10  11  12  13
mapa = [[0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0],
       [0 , 1 , 1 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0],
       [0 , 1 , 1 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0],
       [0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0],
       [0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 1 , 0 , 0],
       [0 , 0 , 0 , 0 , 1 , 1 , 1 , 0 , 0 , 0 , 1 , 0 , 0],
       [0 , 0 , 0 , 0 , 1 , 1 , 1 , 0 , 0 , 0 , 1 , 0 , 0],
       [0 , 0 , 0 , 0 , 1 , 1 , 1 , 0 , 0 , 0 , 1 , 0 , 0],
       [0 , 0 , 0 , 0 , 1 , 1 , 1 , 0 , 0 , 0 , 1 , 0 , 0],
       [0 , 1 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0],
       [0 , 1 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0],
       [0 , 1 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0],
       [0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0],
       [0 , 0 , 0 , 0 , 1 , 1 , 1 , 1 , 0 , 0 , 1 , 1 , 0],
       [0 , 0 , 0 , 0 , 1 , 1 , 1 , 1 , 0 , 0 , 0 , 0 , 0],
       [0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0],
       [0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0],
      ]
def contador_islas(mapa):
    count = 0
    visited = set()
    for i in range(len(mapa)):
        for j in range(len(mapa[0])):
            if (i, j) not in visited and mapa[i][j] == 1:
                count += 1
                stack = [(i, j)]
                while stack:
                    x, y = stack.pop()
                    visited.add((x, y))
                    for dx, dy in [(0, 1), (0, -1), (1, 0), (-1, 0)]:
                        nx, ny = x + dx, y + dy
                        if 0 <= nx < len(mapa) and 0 <= ny < len(mapa[0]) and (nx, ny) not in visited and mapa[nx][ny] == 1:
                            stack.append((nx, ny))
    
    return count

print(contador_islas(mapa))
~~~