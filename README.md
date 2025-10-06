# 🧭 Transport Network Analysis

This project analyzes the **transportation network of Hanoi** using graph theory and network analysis techniques.  
It applies tools from **NetworkX**, **pandas**, and **matplotlib** to uncover the structure of the network, identify key intersections and visualize connectivity patterns.

---

## 🚦 Steps Performed

### 1. Data Loading and Cleaning

- Loaded transportation data and created a directed graph using NetworkX.

- Filtered nodes and edges to remove isolated intersections or incomplete routes.

- Saved the cleaned graph as road_graph.pkl.

### 2. Network Metrics

- Calculated centrality measures:

- In-degree / Out-degree

- Betweenness Centrality

- PageRank

- Authority / Hub Scores

- Generated visualizations:

- Histograms of degree and centrality distributions.

- Scatterplots comparing different measures.

- Correlation heatmap of all centralities.

### 3. Community Detection

- Applied Louvain algorithm to detect densely connected clusters of intersections.

- Exported community data to:

- output/communities.csv

- output/community_analysis.csv

- Visualized community clusters with color-coded nodes.

### 4. Network Visualization

- Used spring layout to plot the largest weakly connected component.

- Nodes sized by betweenness centrality, colored by community.

- Saved high-resolution plot as output/network_graph.png.

### 5. PDF Report Generation

- Generated a report transport_network.pdf summarizing:

- Project overview

- Graph statistics

- Centrality analysis

- Community detection

- Network visualization

- Correlation results

- Discussion and insights

- References



## 📊 Key Insights

- A small number of intersections serve as major transit hubs with high betweenness and PageRank.

- Communities correspond to distinct neighborhoods or sub-networks with dense internal traffic.

- Centrality correlations reveal overlapping but distinct roles of nodes in the network.

## 🧠 Tools and Libraries

- Graph Analysis:	NetworkX, Python-Louvain
- Data Processing:	pandas, numpy
- Visualization:	matplotlib, seaborn
- Report Generation:	fpdf2
- Environment:	Python 3.10+, Jupyter Notebook

## 📘 Results and Outputs

- PDF Report

- Graph Files: .pkl objects for reproducibility

- Visuals: 12+ figures including histograms, scatterplots and heatmaps

- Community Data: CSVs for further exploration

## 🧩 Future Improvements

- Add OpenStreetMap data integration directly via OSMnx.

- Include time-based traffic weighting (rush hour vs. off-peak).

- Automate HTML dashboard generation with Plotly or Dash.

## 📚 References

- NetworkX Documentation

- Blondel, V. D. et al. (2008). Fast unfolding of communities in large networks.

- FPDF2 Documentation

- OpenStreetMap Data

Author: Nick Holden

Project: Transport Network Analysis
License: MIT
Year: 2025
