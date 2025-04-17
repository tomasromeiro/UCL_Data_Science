# Global Meat Trade Network Analysis

**COMP0047 – Data Science**  
**Author: Tomás Romeiro**

---

## Project Overview

This capstone project, developed as part of the COMP0047 Data Science course at University College London, applies advanced network‑analysis techniques to real‑world trade data. Leveraging historical (2005–2022) and forecasted (2023–2040) meat‑trade flows from the Global Trade Atlas dataset, the study uncovers how a handful of countries dominate global supply chains, maps the structure of international trading communities, and evaluates the system’s resilience to major disruptions.

This repository contains the final report and corresponding Python notebook used to produce the analysis, including:

- **Data Cleansing & Transformation**: Tidying time‑series tables into analysis‑ready formats, handling missing values, and separating historical versus forecast segments.
- **Exploratory Analysis**: Summarising overall trade volume, value, and implied price trends; quantifying market concentration on both import and export sides.
- **Network Construction & Pruning**: Building directed graphs of exporter→importer relationships, then filtering edges to retain the top 90% of trade flows.
- **Centrality Metrics & Dependency**: Computing closeness, betweenness, eigenvector centrality, PageRank, and identifying critical (>50%) supplier dependencies.
- **Community Detection**: Revealing regional and cross‑regional trading blocs through modularity‑based clustering.
- **Robustness Simulation**: Demonstrating vulnerability by removing top hubs—both high‑centrality importers and high‑out‑degree exporters—and measuring network fragmentation.
- **Spectral Analysis**: Examining Laplacian eigenvalues to detect latent substructures and confirm overall network resilience.

---

## Main Takeaways

- **Supply‑Chain Risk**: By pinpointing the relatively small group of major exporters (17 countries supplying 80% of meat trade), stakeholders can prioritise diversification and contingency planning.
- **Policy Insights**: Community structures reflect the impact of trade agreements, tariffs, and geography—critical for informed negotiation and logistics optimisation.
- **Technical Showcase**: This project blends Python‑based data‑engineering, statistical summarisation, graph theory, and visualisation—skills highly sought by data‑driven organisations.

---

## Technologies & Techniques

- **Python** (pandas, NumPy, NetworkX, matplotlib, seaborn)  
- **Network Analysis**: Directed and undirected graph construction, centrality measures, community detection  
- **Statistical Methods**: Cumulative distribution, quantile pruning, eigenvalue analysis  
- **Visualisation**: Custom network layouts, treemaps, annotated time‑series plots  

---

## Next Steps & Extensions

- **Dynamic Networks**: Incorporate time‑stepped network evolution to capture shocks (e.g. tariffs, pandemics).  
- **Risk Modelling**: Layer in geopolitical and logistical risk indices to simulate realistic disruption scenarios.  
- **Machine Learning**: Predict emerging exporter hubs or importer dependencies using supervised algorithms.  

---

This project exemplifies the intersection of data science, network theory, and trade economics. It is intended both as a demonstration of COMP0047 course learnings and as a portfolio piece showcasing skills relevant to roles in supply‑chain analytics, risk management, and data-driven policy research.  
