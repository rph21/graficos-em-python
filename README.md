# graficos-em-python
este é  um dos exemplos de um gráfico no python utilizando a biblioteca matplotlib.pyplot 
this is one of the examples of a graph in Python using the matplotlib.pyplot library

import numpy as np
import matplotlib.pyplot as plt
from mpl_toolkits.mplot3d import Axes3D

np.random.seed(42)
num_pontos = 100
x = np.random.randn(num_pontos)
y = np.random.randn(num_pontos)
z = np.random.randn(num_pontos)

fig = plt.figure()
ax = fig.add_subplot(111, projection='3d')

ax.scatter(x, y, z, c='r', marker='o')

ax.set_xlabel('Eixo X')
ax.set_ylabel('Eixo Y')
ax.set_zlabel('Eixo Z')

plt.show()
