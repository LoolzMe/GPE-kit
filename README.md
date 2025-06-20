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

### Data Output

Running the `simulated_annealing/GL_Jax.ipynb` notebook generates simulation results and visualizations, which are saved in the `simulated_annealing/data/` directory. The data is organized into subfolders based on simulation parameters (e.g., `dx=0.25,init=cylinder_symmetry`: `dx` - physical distances between the sites, `init` - initial condition). Each subfolder contains:

- **Numpy arrays** (`.npy`): Final simulation states, e.g., `Delta_final_cylinder_25_884736_0.25.npy`: `Delta_final_{init_condition}_{mu_z}_{number_of_sites}_{dx}.npy`, `mu_z` - magnitude of magnetic dipole in dimensionless units, `number_of_sites` - number of sites used in simulation, `dx` - physical distances between the sites.
- **HTML reports** (`.html`): Interactive summaries of the results (3d model of isosurface of 0.5 density)
- **PNG images**: Slices and visualizations of the simulation, such as `x-slice.png`, `y-slice.png`, `velocity_field_z_slice.png`, and residual plots
