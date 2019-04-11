# ioe691-project
This repository contains the example files (in Julia) that were used to compare the ability of Diagonally Dominant Sums of Squares (DSOS) polynomials to replace Sums of Squares (SOS) polynomials within a certain problem class: Stability Number Calculation. Mostly written in Julia, this contains multiple notebooks outlining our examples.

## Description of Each Notebook
Each notebook contains the optimization problem needed to identify the stability number of a given graph (the graph is the primary thing that changes between notebooks). Note that the notebook `Recreating DSOS Stable Set Example.ipynb` contains the mathematical description of what optimization problem is solved and why. The other files simply use the same operations/method.

Within each notebook, a new graph is analyzed. For quick reference, these are the graphs and associated notebooks.
* Isocahedron (Stability Number = 3), analyzed in `Recreating DSOS Stable Set Example.ipynb`
* Generalized Peterson Graph GP(6,1) (Stability Number = 6), analyzed in `SOS-DSOS Comparison Example 4.ipynb`
* Generalized Peterson Graph GP(7,2) (Stability Number = 5), analyzed in `SOS-DSOS Comparison Example 5.ipynb`

A quick warning is offered to the viewer of these notebooks. In practice, it appears that it is very hard for Julia to optimize over r-DSOS and r-SDSOS polynomials when r>2 for the problems that we analyze here. If the user modifies r in the included notebooks, the optimization may not be solved.