# Proyecto A* Pathfinding - Navegación Autónoma
Este proyecto forma parte del módulo de Programación de Inteligencia Artificial.

## 1. Fase de Investigación
El algoritmo A* es un algoritmo de búsqueda de caminos que encuentra la ruta más corta entre un nodo de origen y uno de destino. Utiliza la fórmula:
$f(n) = g(n) + h(n)$
Donde:
- **g(n)**: Coste del camino desde el inicio.
- **h(n)**: Heurística (estimación hasta la meta).

## 2. Comparativa de Algoritmos
- **A* vs Dijkstra**: A* es más eficiente porque usa la heurística para "guiarse", mientras que Dijkstra explora en todas direcciones.
- **A* vs BFS**: BFS encuentra la ruta con menos pasos en mapas sin costes, pero A* es superior cuando hay diferentes terrenos o distancias reales.
