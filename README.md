# Graph Coloring Python

Python code and Jupyter notebooks accompanying my work in graph theory.

## Notebooks

* **`equitable-colorings.ipynb`** — Algorithms for equitable colorings of sparse graphs, including computational experiments related to [*Equitably Coloring Planar and Outerplanar Graphs*](https://arxiv.org/abs/2509.16123), by Daniel W. Cranston and Reem Mahmoud.
  
* **`correspondence-packing.ipynb`** — Algorithms for 5-choosability of planar graphs and packing 3 correspondence colorings, given any K<sub>5</sub>-minor free graph and a correspondence 6-cover.  Includes a nice visualization for converting Thomassen's proof to a coloring algorithm that is very efficient!  Related to [*Disjoint Correspondence Colorings for K5-Minor-free Graphs*](https://arxiv.org/abs/2602.16692) by Wouter Cames van Batenburg, Daniel W. Cranston, and František Kardoš.

* **`sparse-recoloring.ipynb`** - Algorithms for reconfiguration of list-colorings in sparse graphs.  Given a graph $G$, list assignment $L$, and $L$-colorings $\alpha,\beta$, a reconfiguration sequence transforms $\alpha$ to $\beta$ by recoloring one vertex at a time, so
that each intermediate coloring is also a proper coloring.  A key tool for growing a reconfiguration sequence for $G-v$ to one for $G$ is the so-called *Extension Lemma*, which we implement here.  A naive implementation runs in time $\Theta(n^2)$.  But by using a custom type of treap as our data structure, we reduce this to time $O(n\log n)$.  This allows us to handle much larger graphs.  Based on this technical advance, we then implement two of the main results for the paper, and test them on large graphs.

## Author

Daniel W. Cranston

For more information about my research and publications, see [graphcoloringmethods.com/writing.html](https://graphcoloringmethods.com/writing.html).

