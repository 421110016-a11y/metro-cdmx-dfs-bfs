# Metro CDMX — Búsqueda de rutas con DFS y BFS

## Descripción

Este proyecto modela la red del Metro de la Ciudad de México como un grafo
y utiliza los algoritmos de búsqueda no informada DFS (Depth-First Search)
y BFS (Breadth-First Search) para encontrar rutas entre diferentes estaciones.

Cada estación del Metro se representa como un nodo y cada conexión entre
estaciones consecutivas como una arista.

Para este proyecto se utiliza un costo unitario:

**Moverse de una estación a otra tiene un costo de 1.**

## Rutas analizadas

1. Cuatro Caminos → Pantitlán
2. Politécnico → Tasqueña
3. Zapata → Oceanía

## Algoritmos utilizados

### DFS — Depth-First Search

DFS realiza una búsqueda en profundidad utilizando una estructura tipo pila
(LIFO). Permite encontrar una ruta entre dos estaciones, aunque no garantiza
que sea la ruta con el menor número de movimientos.

### BFS — Breadth-First Search

BFS realiza una búsqueda por niveles utilizando una cola (FIFO).

Como todas las conexiones tienen costo 1, BFS permite encontrar una ruta
con el menor número de movimientos entre el origen y el destino.

## Resultados

| Ruta | Algoritmo | Movimientos | Nodos explorados |
|---|---|---:|---:|
| Cuatro Caminos → Pantitlán | DFS | 18 | 19 |
| Cuatro Caminos → Pantitlán | BFS | 18 | 123 |
| Politécnico → Tasqueña | DFS | 46 | 94 |
| Politécnico → Tasqueña | BFS | 20 | 146 |
| Zapata → Oceanía | DFS | 22 | 47 |
| Zapata → Oceanía | BFS | 13 | 113 |

## Tecnologías utilizadas

- Python
- NetworkX
- Matplotlib
- Pandas
- Google Colab
- GitHub

## Autor

Luis Ángel Ciprés Flores
