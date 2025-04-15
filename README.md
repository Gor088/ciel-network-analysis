Graph analysis of the Ciel drug network.

# Project Ciel: Graph Theory and Network Analysis

This project analyzes a real-world criminal network using graph theory and network analysis techniques. The data is based on **Project Ciel**, an investigation into a drug-importation operation smuggling liquid hashish from Jamaica to Montreal in the late 1990s. Out of 75 people, 25 were identified as active participants in the drug-importation operations.

## 🧠 Objective

To analyze the structure and dynamics of this criminal network by:
- Visualizing the network graph and exploring its layout
- Identifying key individuals using centrality measures such as degree, betweenness, and closeness centrality
- Calculating global properties such as network density and global clustering coefficient
- Ranking participants based on influence and connectivity
- Plotting degree centrality (x-axis) against betweenness centrality (y-axis) with node labels and average-based dividing lines to identify four communication behavior regions
- Visualizing the deviations of each node's centrality values (degree, betweenness, closeness) from their respective averages to detect outliers and potential leaders

## 🛠️ Methods & Tools

- **Python Libraries:** NetworkX, Pandas, NumPy, Matplotlib, Plotly
- **Graph Metrics:**
  - Degree Centrality
  - Betweenness Centrality
  - Closeness Centrality
  - Clustering Coefficient
  - Network Density
  - Global Clustering Coefficient

## Network Analysis Summary

The Ciel network is sparse, as most nodes have low degree centrality and there are few connections relative to the total number of possible edges in a 25-node undirected graph. This sparsity suggests the network is intentionally designed to reduce exposure and compartmentalize operations.

From the results of our centrality measures:
- **Node 2** is the ring leader with the highest degree, betweenness, and closeness centrality.
- **Node 1** acts as the lieutenant, supporting Node 2 and holding the second-highest scores.
- The network is highly centralized around **Nodes 2 and 1**, who serve as communication and control hubs.
- **Node 13** also plays a significant role in communication flow and is closely tied to the core leadership (Node 1 being a key part of that leadership).

We identify:
- **Key players (action segment):** Nodes 1, 2, and 13.
- **Drug mules (low centrality nodes):** Nodes 5, 6, 12, 14, 15, 16, 18, 19, 20, 21, 23, 25.
- **Complimentary segment:** Nodes 4, 7, 8, 10, 11, 13, 3, 9, 15, 17, 22, 24.

Removing **Nodes 2, 1, and 13** would dismantle the network by disrupting its core communication and organizational structure.

