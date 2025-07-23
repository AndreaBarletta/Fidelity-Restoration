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
