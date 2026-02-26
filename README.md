# ⚓ Proyecto A* Pathfinding - Navegación Autónoma Ártica

Este proyecto ha sido desarrollado para el módulo de **Programación de Inteligencia Artificial**. Consiste en un simulador de navegación donde un buque debe hallar la ruta óptima en un entorno dinámico con obstáculos (icebergs).

## 1. Fase de Investigación
El algoritmo **A*** es un método de búsqueda de caminos que garantiza encontrar la ruta más corta de manera eficiente. Se basa en la función de evaluación:

$$f(n) = g(n) + h(n)$$

* **$g(n)$**: Coste real del camino recorrido desde el origen.
* **$h(n)$**: Heurística (distancia estimada hasta la meta). En este simulador se utiliza la distancia euclidiana para permitir movimientos precisos en 8 direcciones.



## 2. Implementación y Diseño
* **Interfaz de Usuario (UX):** Se ha diseñado un menú interactivo mediante `IPyWidgets`. Para optimizar la ergonomía y la disposición de los controles, **se ha contado con asistencia de IA**, logrando un panel compacto que permite ajustar el tamaño del mapa y la densidad de icebergs en tiempo real.
* **Portabilidad y Automatización:** El sistema es "plug-and-play". Incluye un script que sincroniza automáticamente los recursos gráficos (`barco.webp`) desde este repositorio, asegurando que la simulación funcione correctamente en Google Colab sin necesidad de subir archivos manualmente.

## 3. Comparativa de Algoritmos
* **A* vs Dijkstra:** A diferencia de Dijkstra, que explora en todas direcciones de forma uniforme, A* utiliza la heurística para priorizar los nodos que se acercan al destino, reduciendo drásticamente el tiempo de computación.
* **A* vs BFS:** BFS es efectivo para encontrar el camino con menos pasos en grafos simples, pero no gestiona distancias reales ni costes. A* es superior en este contexto al procesar correctamente los movimientos diagonales y distancias euclidianas.

---
**Autor:** Antonio Guisado  
**Entorno:** Python 3.0 / Google Colab
