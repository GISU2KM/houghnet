# HoughNet

Code the paper

[Implicit Hough Transform Neural Networks for Subspace Clustering](...)  
Julian Busch, Maximilian Hünemörder, Janis Held, Peer Kröger, and Thomas Seidl  
2021

## Setup
Install the required packages specified in the file `requirements.txt`, e.g., using `pip install -r requirements.txt`. Additionally, the package `torch==1.8.1` is required and can be installed depending on your system and CUDA version following this guide: [https://pytorch.org/get-started/locally/](https://pytorch.org/get-started/locally/).

## Demo
We provide a demonstration of how to use this code in the notebook `src/demo.ipynb`.

## Running Experiments
- To run experiments or to reproduce the results reported in the paper, you can use the script `src/run_experiment.py`.
- Parameters need to be specified in a config-file in *JSON*-syntax. We uploaded config-files containing the default parameter-values used in our experiments into the folder `config`.
- The remaining parameters were optimized using a grid search. A grid search can be started with the script `src/run_grid_search.py`. The used parameter grids are stored in that file.
- Results will be tracked by *MLflow*. By default, results will be stored in the local file system.
