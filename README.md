# Dijkstra Algorithm Visualizer

An interactive web application built with Streamlit to visualize the Dijkstra shortest path algorithm step by step. The application allows users to input a graph structure, select a starting node, and observe how the algorithm explores nodes, updates distances, and determines the shortest paths.

---

## Features

- Interactive graph input using Python dictionary format.
- Step-by-step visualization of Dijkstra's Algorithm.
- Real-time shortest distance calculation from a selected source node.
- Graph visualization using NetworkX and Matplotlib.
- Highlight visited nodes and explored edges.
- Detailed execution logs for every iteration.
- Supports custom weighted graphs.

---

## Algorithm

The application implements the **Dijkstra Shortest Path Algorithm**, which finds the minimum distance from a source node to all other nodes in a weighted graph with non-negative edge weights.

During execution, the application:

1. Selects the node with the smallest tentative distance.
2. Updates neighboring node distances.
3. Marks visited nodes.
4. Visualizes explored edges and current node.
5. Displays detailed logs for each step.

---

## Technologies Used

- Python
- Streamlit
- NetworkX
- Matplotlib
- Heapq
- Pillow (PIL)

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/dijkstra-visualizer.git
cd dijkstra-visualizer
```

Install dependencies:

```bash
pip install -r requirements.txt
```

or

```bash
pip install streamlit networkx matplotlib pillow
```

---

## Running the Application

Run the Streamlit app:

```bash
streamlit run app.py
```

The application will open automatically in your browser.

---

## Input Format

Graphs must be entered as a Python dictionary.

Example:

```python
{
    '0': {'1': 2, '2': 6},
    '1': {'0': 2, '3': 5},
    '2': {'0': 6, '3': 8},
    '3': {'1': 5, '2': 8, '4': 10, '5': 15},
    '4': {'3': 10, '6': 2},
    '5': {'3': 15, '6': 6},
    '6': {'4': 2, '5': 6}
}
```

Then enter the starting node and click **Jalankan Dijkstra**.

---

## Example Output

The application displays:

- Shortest distances from the source node
- Visual graph for every iteration
- Visited nodes and traversed edges
- Detailed execution logs

---

## Project Structure

```text
.
├── app.py
├── requirements.txt
└── README.md
```

---

## Educational Purpose

This project was developed as a learning tool for understanding graph traversal and shortest path algorithms through interactive visualization.

---

## Author

Wa Ode Zachra Chaerani
