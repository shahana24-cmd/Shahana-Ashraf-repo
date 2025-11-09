# 🧩 DSC212: Modularity on the Karate Club Graph

This repository contains the implementation of **Recursive Spectral Modularity Partitioning**
for community detection on the classic **Zachary’s Karate Club graph**.

## 📘 Course
**DSC212: Graph Theory Module**

## 🧑‍💻 Author
Your Name  
IISER Thiruvananthapuram  

---

## 📄 Description
This project implements **modularity-based community detection** using the **spectral method**:
- Computes the **modularity matrix** B = A - (kkᵀ)/(2m)
- Finds the **leading eigenvector** to determine the best graph split
- Performs **recursive bisection** until modularity gain is nonpositive
- Calculates **node centrality metrics** at each stage:
  - Degree centrality
  - Betweenness centrality
  - Closeness centrality
  - Clustering coefficient
- Visualizes community splits and metric evolution across iterations

---

## 🧰 Dependencies
The code uses standard Python scientific libraries:

```
networkx
numpy
matplotlib
pandas
```

You can install them using:
```bash
pip install -r requirements.txt
```

---

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/DSC212-Modularity-KarateClub.git
   cd DSC212-Modularity-KarateClub
   ```
2. Open the notebook:
   ```bash
   jupyter notebook DSC212_KarateClub_Modularity.ipynb
   ```
3. Run **all cells** (Kernel → Restart & Run All).  
   The notebook runs **top-to-bottom without manual edits**.

---

## 🖼️ Visualizations
The notebook automatically displays:
- Graph visualizations after each spectral split
- Metric evolution plots for all nodes

---

## 📚 Reference
Newman, M. E. J. (2006). *Modularity and community structure in networks.*  
PNAS 103(23): 8577–8582.

---

## 🏁 Output
The notebook detects multiple communities in the Karate Club network and confirms that the split aligns closely with the real division observed between *Mr. Hi’s group* and the *club president’s group*.
