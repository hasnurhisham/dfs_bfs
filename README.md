BFS & DFS Search Algorithms Web Application (Streamlit)

A web-based interactive application built with Streamlit, Python, NetworkX, and Matplotlib to visualize, step through, and analyze the execution of Uninformed Search Algorithms—Breadth-First Search (BFS) and Depth-First Search (DFS)—on directed graphs.

Developed as part of the assessment for BSD3513: Introduction to Artificial Intelligence at Universiti Malaysia Pahang Al-Sultan Abdullah (UMPSA).

🔗 Project Links

* **Live Streamlit App:** https://lab-report1-dfs-bfs.streamlit.app 
* **GitHub Repository:** https://github.com/hasnurhisham/dfs_bfs.git 


📌 Problem Overview (Lab 1 Requirements)

This project satisfies the graph search requirements of Lab Report 1 (Question 2 & Question 3):

Graph Traversal Modeling: Supports directed graph parsing with custom node-edge connections and isolated nodes.

Deterministic Tie-Breaking: Enforces strict alphabetical tie-breaking rules across all neighbor expansions.

Dual Uninformed Search Support:

Breadth-First Search (BFS): Level-by-level exploration using a FIFO queue to guarantee minimum-hop paths in unweighted graphs.

Depth-First Search (DFS): Deep path exploration using a LIFO stack (with reverse-alphabetical pushing to prioritize alphabetical visitation).

Step-by-Step State Trace: Full inspection of node visits, queue/stack state changes, depth tracking, and parent pointers.

✨ Features

Dynamic Graph Editor: Edit directed edge definitions directly from the Streamlit sidebar (e.g., A B, B E).

Interactive Step Inspection: Interactive slider to step through node expansion step-by-step.

Network Graph Visualization: Color-coded network diagrams highlighting the active node, discovered nodes, and unvisited nodes using NetworkX and Matplotlib.

Quantitative Search Metrics: Displays total expanded nodes, maximum recorded frontier size, and goal path edge count.

Full Step Trace Log: Interactive pandas DataFrame rendering the queue/stack frontier state, depth, parent links, and visited nodes for every step.

🛠️ Project Structure

├── dfs_bfs.py            # Main Streamlit application and search algorithms logic
├── requirements.txt      # Required dependencies for Streamlit Community Cloud
└── README.md             # Project documentation


🚀 Local Setup & Installation

Follow these steps to run the application locally on your machine:

1. Clone the Repository

git clone https://github.com/hasnurhisham/BFS-DFS-Lab1.git
cd BFS-DFS-Lab1


2. Set Up Virtual Environment (Optional but Recommended)

# macOS/Linux
python3 -m venv venv
source venv/bin/activate

# Windows
python -m venv venv
venv\Scripts\activate


3. Install Dependencies

pip install -r requirements.txt


4. Run the Streamlit App

streamlit run dfs_bfs.py


📦 Dependencies (requirements.txt)

Ensure your repository contains a requirements.txt file with the following packages:

streamlit
pandas
networkx
matplotlib


📊 Experimental Results & Traversal Verification

When evaluated on the lab graph topology starting from Node A targeting Goal Node F:

Breadth-First Search (BFS)

Expansion Order: $A \rightarrow B \rightarrow D \rightarrow C \rightarrow E \rightarrow G \rightarrow H \rightarrow F$

Goal Path Found: $A \rightarrow B \rightarrow G \rightarrow F$

Expanded Nodes: 8

Max Recorded Frontier: 4

Goal Path Edges: 3

Depth-First Search (DFS)

Expansion Order: $A \rightarrow B \rightarrow C \rightarrow E \rightarrow H \rightarrow F$

Goal Path Found: $A \rightarrow B \rightarrow E \rightarrow H \rightarrow F$

Expanded Nodes: 6

Max Recorded Frontier: 4

Goal Path Edges: 4

