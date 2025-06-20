# GPE-kit
Gross-Pitaevsky solutions kit written mainly in Python.
Overleaf project files are [here](https://www.overleaf.com/read/gqzmzzdczbyb#5b8d5b)

## Simulated annealing

### Jupyter Notebooks

The project includes Jupyter notebooks for interactive development and analysis:

- `simulated_anneling/GL_Jax.ipynb`: A notebook implementing the Ginzburg-Landau equation solver using JAX for automatic differentiation and optimization. This notebook contains the implementation of simulated annealing algorithm for finding ground state solutions. It also contains residue calculation (substition into GL equation) in order to access the correctness of the solution.

To run the notebooks:
1. Ensure you have Jupyter installed (`pip install jupyter`)
2. Navigate to the project directory
3. Run `jupyter notebook` to start the Jupyter server
4. Open the desired notebook in your browser
5. Run the notebook, run all won't likely work.
