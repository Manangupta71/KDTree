# 🌳 KDTree Lab — KNN Benchmark & Visualization

An interactive visualization and benchmarking tool that demonstrates the performance difference between **KD-Tree** and **Brute Force** approaches for solving the **K-Nearest Neighbors (KNN)** problem.

🔗 Live Demo: https://manangupta71.github.io/KDTree/

---

## 📌 Overview

This project provides a hands-on, visual understanding of how **data structures impact machine learning performance**.

It compares:

* **KD-Tree (O(log n))**
* **Brute Force (O(n))**

through real-time benchmarks, interactive queries, and scaling analysis.

---

## 🚀 Features

### 🔹 Interactive Visualization

* Click anywhere on the canvas to perform a KNN query
* Visualizes:

  * Query point
  * Nearest neighbors
  * KD-tree traversal path

### 🔹 Real-Time Benchmarking

* Compare:

  * KD-Tree query time
  * Brute-force query time
* Displays:

  * Speedup factor
  * Nodes visited
  * Accuracy comparison

### 🔹 Adjustable Parameters

* Dataset size (50 → 5000)
* Number of neighbors (K)
* Dimensions (2D → 32D)

### 🔹 Scaling Analysis

* Performance vs dataset size
* Graph visualization using Chart.js
* Demonstrates:

  * O(log n) vs O(n) growth

### 🔹 KD-Tree Visualization

* Recursive tree structure rendering
* Axis-based splitting (x-axis / y-axis)

---

## 🧠 Concepts Covered

* KD-Tree construction
* Recursive space partitioning
* Nearest neighbor search optimization
* Backtracking in tree traversal
* Curse of dimensionality
* Time complexity comparison

---

## ⚙️ Tech Stack

* HTML5 + CSS3
* Vanilla JavaScript
* Canvas API (for visualization)
* Chart.js (for performance graphs)

---

## 🏗️ Implementation Details

### KD-Tree

* Built recursively by splitting on median values
* Axis selection based on depth (`axis = depth % dimensions`)
* Efficient pruning using distance comparison

### KNN Search

* Maintains a max-heap of nearest neighbors
* Traverses:

  * Near subtree first
  * Then far subtree if required

### Brute Force

* Computes distance from query to all points
* Sorts and selects top K neighbors

---

## 📊 Key Observations

* KD-Tree significantly reduces search space
* Performance improves as dataset size increases
* Accuracy remains comparable to brute force
* Efficiency drops in high dimensions (curse of dimensionality)

---

## 📁 Project Structure

```
KDTree/
│── index.html   # Main application (UI + logic)
│── README.md    # Documentation
```

---

## ▶️ How to Run

### Option 1: Live

Just open:
👉 https://manangupta71.github.io/KDTree/

### Option 2: Local

```bash
git clone https://github.com/Manangupta71/KDTree.git
cd KDTree
open index.html
```

---

## 🎯 Use Cases

* Data Structures learning (KD-Trees)
* Machine Learning fundamentals (KNN optimization)
* Interview preparation (DSA + ML intersection)
* Visualization of algorithm behavior

---

## 💡 Future Improvements

* Add 3D visualization
* Support real datasets (CSV upload)
* Implement Ball Tree / ANN comparison
* GPU acceleration for large datasets

---

## 👨‍💻 Author

**Manan Gupta**
BTech CSE @ NIT Hamirpur

---

## ⭐ If you found this useful

Give this repo a star ⭐ — helps a lot!

---
