# 🌾 AgriGuard – Crop Disease Quarantine Zone Management System

**Analyze Connections. Identify Critical Farms. Plan Smarter Quarantine Zones.**

AgriGuard is a console-based **Java** mini-project built with ADS & AA concepts. It models farms as vertices and possible disease-contact pathways as edges in an undirected graph, then finds connected groups, critical farms and potential quarantine zones.

## 👥 Team Members

| S. No. | Name | Role |
|--------|------|------|
| 1 | G. Malleswari | Team Leader |
| 2 | P. Bhuvana Sri | Team Member |
| 3 | S. L. S. Venkat Reddy | Team Member |

## 🎯 Objectives

- Represent farms and contact pathways as a graph.
- Find connected groups of farms using BFS and DFS.
- Detect critical farms and biconnected components.
- Rank farms by their impact on connectivity.
- Simulate quarantine and support adding/removing connections.

## ✨ Key Features

1. Graph representation (farms = vertices, contacts = undirected edges)
2. Add or remove connections dynamically
3. BFS and DFS traversal for connected components
4. Articulation point detection (Tarjan's algorithm)
5. Biconnected components
6. Critical farm ranking
7. Quarantine simulation
8. Sample networks (chain, star, cyclic)
9. Complexity analysis

## 🧠 Data Structures and Algorithms

| Concept | Application |
|---------|-------------|
| Adjacency List | `List<TreeSet<Integer>>` stores farm connections |
| TreeSet | Unique, sorted neighbours |
| Queue (`LinkedList`) | BFS traversal |
| Stack (`ArrayDeque`) | Biconnected components |
| BFS / DFS | Connected components |
| Tarjan's Algorithm | Articulation points |

## 🛠️ Technology Stack

Java 8 or later (JDK) | Eclipse / IntelliJ / NetBeans / VS Code | `javac` | No external libraries

## ⚙️ Run the Project

```bash
git clone https://github.com/YOUR-USERNAME/AgriGuard.git
javac AgriGuard.java
java AgriGuard
```

The same commands work on Windows, Linux and macOS.

## 🧪 Test Scenarios

| Network | Structure | Expected Result |
|---------|-----------|-----------------|
| Chain | 1-2-3-4-5 | Critical farms: 2, 3, 4 |
| Star | Farm 1 connected to all | Critical farm: 1 |
| Cyclic | 1-2-3-4-5-1 | No critical farms |

## 📊 Algorithm Complexity

| Algorithm | Time | Space |
|-----------|------|-------|
| BFS | O(V + E) | O(V) |
| DFS | O(V + E) | O(V) |
| Articulation Points | O(V + E) | O(V) |
| Biconnected Components | O(V + E) | O(V + E) |
| Critical Farm Ranking | O(V(V + E) + V log V) | O(V) |
| Quarantine Simulation | O(V + E) | O(V) |

V = number of farms, E = number of contact pathways.

## 🌱 Real-World Application

When a disease is reported on a farm, the system can show which farms are connected to it, divide the network into groups, find critical connection points, and simulate isolating a farm.

> **Note:** AgriGuard is an educational prototype. It shows structural connectivity only and does not predict infection, transmission probability or outbreak risk.

## 📁 Project Structure

```
AgriGuard/
├── AgriGuard.java
├── README.md
├── IDEOLOGY.md
├── ALGORITHM.md
├── REQUIREMENTS.md
├── screenshots/
└── test_cases/network_test_cases.md
```

## 🚀 Future Enhancements

Weighted connections, risk-based prioritization, file save/load, graph visualization (Swing/JavaFX), map integration and disease-spread models.

## 🎓 Academic Relevance

Covers graph traversal, BFS, DFS, articulation points, biconnected components, complexity analysis and dynamic graph operations.

## 🤝 Team Contribution & 📜 License

Developed collaboratively as an academic mini-project, for academic and educational purposes.

---

**AgriGuard – Analyze Connections. Identify Critical Farms. Plan Smarter Quarantine Zones.** 🌾
