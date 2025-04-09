# District Graph Coloring

This project implements graph coloring algorithms to solve the **district coloring problem**, which is the assignment of colors to districts such that no two adjacent districts share the same color. This is useful in areas like geographical zoning, network segmentation, and scheduling.

## 🌍 Project Highlights

- **Dataset Source**: A set of districts and their connections (adjacency) from a `.xlsx` file.
- **Graph Construction**: Each district is treated as a node, and edges denote adjacency.
- **Algorithms Implemented**:
  - Greedy Coloring
  - Welch-Powell Coloring

## 🔧 Technologies Used

- Python
- Pandas
- NetworkX
- Matplotlib

## 📊 Dataset Overview

The dataset contains pairs of districts represented by their `a_i` and `a_j` codes, each pair forming an edge.

| Kode Kalurahan | Kalurahan   | a_i | a_j |
|----------------|-------------|-----|-----|
| 1              | Argodadi    | 1   | 3   |
| 2              | Argomulyo   | 1   | 4   |
| ...            | ...         | ... | ... |

## 🧠 Graph Coloring Explained

### 🎨 Greedy Coloring

- Assigns the smallest possible color to each node.
- Processes nodes in default order.

### 🏆 Welch-Powell Coloring

- Sorts nodes by degree (most connected first).
- Typically yields fewer colors than Greedy.

## 📈 Visualization

Visualizes nodes (districts) and their assigned colors using `spring_layout`.

- **Greedy Coloring Result:** 3 colors
- **Welch-Powell Coloring Result:** 3 colors

## 🧪 Sample Result

```python
Greedy Coloring: {1: 0, 3: 1, 4: 2, 2: 0, 6: 1, ...}
Welch Powell Coloring: {6: 0, 17: 0, 10: 0, 14: 0, ...}
```

## ✅ Conclusion

Both algorithms successfully assign colors using only 3 different values. Welch-Powell often performs better in complex graphs. Graph coloring is a powerful tool for ensuring adjacent entities do not conflict in resource allocation, zoning, or scheduling tasks.

---

*Made with ❤️ by Alexander Tiopan*

