# BSD3513 Artificial Intelligence — Lab Report 1
**Interactive Uninformed Search Algorithms (BFS & DFS)**


## 📌 Project Overview
This repository contains the interactive web application prototype developed for **BSD3513 Introduction to Artificial Intelligence (Lab Report 1)** at **Universiti Malaysia Pahang Al-Sultan Abdullah (UMPSA)**. 

The application visualizes and compares two fundamental uninformed search algorithms:
* **Breadth-First Search (BFS):** Level-by-level state-space traversal using a First-In, First-Out (FIFO) queue data structure.
* **Depth-First Search (DFS):** Deep path state-space traversal using a Last-In, First-Out (LIFO) stack data structure with tie-breaking rules.

---

## 🔗 Live Application & Links
* **Live Streamlit App:** https://lab-report1-dfs-bfs.streamlit.app 
* **GitHub Repository:** https://github.com/hasnurhisham/dfs_bfs.git 

---

## ✨ Features
* 📊 **Dynamic Graph Parsing:** Input customized directed graphs directly via an intuitive sidebar editor.
* 🔤 **Alphabetical Tie-Breaking:** Enforces strict alphabetical order for queue insertion (BFS) and reverse-alphabetical order for stack pushing (DFS).
* 🔍 **Step-by-Step Step Inspection:** Interactive slider to step through the traversal process node-by-node.
* 📈 **Real-Time Visualizations & Metrics:**
  * Interactive network layout highlighting current, visited, and frontier nodes.
  * Quantitative metrics: Total expanded nodes, maximum frontier size, and goal path edge count.
  * Complete step trace log showing current state, frontier status, depth, and parent node history.

---

## 🛠️ Installation & Local Setup

### Prerequisites
Make sure you have Python 3.9+ installed on your machine.

### 1. Clone the Repository
```bash
git clone [https://github.com/YOUR_USERNAME/BSD3513-Lab1-BFS-DFS.git](https://github.com/YOUR_USERNAME/BSD3513-Lab1-BFS-DFS.git)
cd BSD3513-Lab1-BFS-DFS
