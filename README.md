# Matrix Decomposition with Fidelity Restoration

This project explores and compares matrix decomposition methods for photonic circuits, with a focus on **fidelity restoration** in the presence of losses and parameter noise. We evaluate our approach against traditional methods like **Reck's** and **Clements'** decompositions.

## Features

- Implements standard Reck and Clements decompositions
- Introduces a fidelity-restoring decomposition method
- Simulates losses and parameter errors
- Compares fidelity performance under noise

## Requirements

- Python 3.8+
- numpy
- matplotlib (optional, for plots)

To install dependencies:

```bash
pip install numpy matplotlib
```

## How to Run

The main program is in the Jupyter notebook:

```bash
jupyter notebook main.ipynb
```

> If you don't have Jupyter installed:
> ```bash
> pip install notebook
> ```

for more intructions, visit the [Jupyter website](https://jupyter.org/)

## File Structure

```
.
├── notebook.ipynb    # Main notebook with all experiments
├── circuit/          # Contains the implementation of the interferometric circuits, both for the math part and the drawing part
└── images/           # Contains all the circuits
```

## Credits
The circuit draw function and interferometer class are an adaptation of the code by Clements et al., available at https://github.com/clementsw/interferometer
In particular we added the support for:
  - more components (phase shifters, losses)
  - possibility to introduce non-idealities in the computation of the transfer function
  - improvements to modularity in the drawing, for example the possiblity to introduce barriers to align components

## References

[1] Reck, Michael, et al. "Experimental realization of any discrete unitary operator." Physical review letters 73.1 (1994): 58. <br>
[2] Clements, William R., et al. "Optimal design for universal multiport interferometers." Optica 3.12 (2016): 1460-1465.<br>
[3] Tsakyridis, A., Giamougiannis, G., Totovic, A. and Pleros, N. (2022), Fidelity Restorable Universal Linear Optics. Adv. Photonics Res., 3: 2200001. https://doi.org/10.1002/adpr.202200001<br>
[4] P. Dita, J. Phys. A: Math. Gen. 2006, 36, 2781. <br>
