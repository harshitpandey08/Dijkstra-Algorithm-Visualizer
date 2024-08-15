# Dijkstra's Algorithm Visualizer

## Overview

**Dijkstra's Algorithm Visualizer** is a Python project designed to demonstrate Dijkstra's shortest path algorithm. This tool computes and visually represents the shortest path between landmarks on a graph. Using the powerful libraries **NetworkX** for graph handling and **Matplotlib** for visualization, it provides an interactive and educational experience for users interested in algorithms and data visualization.

## Features

- **Shortest Path Calculation**: Implements Dijkstra's algorithm to find the shortest path between a start and end node.
- **Interactive User Input**: Users can input their start and destination points to calculate the shortest route.
- **Graph Visualization**: The graph is rendered with visual distinctions for the shortest path, start node, and end node.
- **Customizable Graph**: Easily modify the predefined graph to include more nodes and edges.

## Technologies Used

- **Python 3.x**
- **NetworkX**: For graph creation and manipulation
- **Matplotlib**: For visualizing the graph


1. **Input Nodes**: The program will prompt you to enter a start node and an end node. For example:

    ```text
    Enter your pick up point: HAWA MAHAL
    Enter your destination point: BIRLA MANDIR
    ```

2. **Visualize the Shortest Path**: The program will compute the shortest path and display it along with the graph visualization.

## Example Graph

Here is a sample graph that the algorithm works on:

```python
graph = {
    'HAWA MAHAL': {'AMBER FORT': 2, 'JAL MAHAL': 5},
    'AMBER FORT': {'HAWA MAHAL': 2, 'JAL MAHAL': 1, 'JANTR MANTR': 22},
    'JAL MAHAL': {'HAWA MAHAL': 5, 'AMBER FORT': 1, 'JANTR MANTR': 5},
    'JANTR MANTR': {'AMBER FORT': 22, 'JAL MAHAL': 5, 'BIRLA MANDIR': 4},
    'BIRLA MANDIR': {'JANTR MANTR': 4, 'JAL MAHAL': 8},
}
```

## Visualization

The graph visualization distinguishes:

- **Shortest Path**: Highlighted in green
- **Start Node**: Marked in orange
- **End Node**: Marked in red

## Customization

You can easily expand the graph by modifying the `graph` dictionary in the script. Add more nodes and edges to visualize different scenarios or larger graphs.
