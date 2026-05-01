# Calculus Learning Project

A collection of interactive Jupyter notebooks for learning calculus concepts with Python visualizations.

## Contents

- [01_Limits.ipynb](01_Limits.ipynb) - Foundation of calculus, epsilon-delta definition, special limits
- [02_Functions.ipynb](02_Functions.ipynb) - Functions, domains, ranges, and compositions
- [03_Exponents_and_Logarithms.ipynb](03_Exponents_and_Logarithms.ipynb) - Exponential and logarithmic functions
- [04_Essential_Math_Rules.ipynb](04_Essential_Math_Rules.ipynb) - Key mathematical rules and identities
- [05_Differentiation.ipynb](05_Differentiation.ipynb) - Derivatives and differentiation techniques
- [06_Integration.ipynb](06_Integration.ipynb) - Integrals and integration methods

## Setup Instructions

### 1. Clone the repository

```bash
git clone <your-repo-url>
cd math
```

### 2. Create and activate virtual environment

**macOS/Linux:**
```bash
python3 -m venv venv
source venv/bin/activate
```

**Windows:**
```bash
python -m venv venv
venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install --upgrade pip
pip install -r requirements.txt
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

This will open your browser with the Jupyter interface where you can access all notebooks.

## Best Practices for Workspace Management

### Environment Management

1. **Always use virtual environments** - Isolates project dependencies
2. **Keep requirements.txt updated** - Run `pip freeze > requirements.txt` after installing new packages
3. **Use specific version numbers** - Ensures reproducibility across machines

### Git Workflow

1. **Commit regularly** with meaningful messages
2. **Don't commit large files** - Use `.gitignore` for data files, models, etc.
3. **Jupyter notebooks and git**:
   - Consider using [nbstripout](https://github.com/kynan/nbstripout) to remove output before committing
   - Or manually clear outputs: Cell > All Output > Clear

### Jupyter Best Practices

1. **Restart kernel regularly** - Ensures reproducibility (Kernel > Restart & Run All)
2. **Keep notebooks focused** - One topic per notebook
3. **Document your code** - Use markdown cells to explain concepts
4. **Version control** - Save important versions before major changes

### Project Structure

```
math/
├── README.md              # Project documentation
├── requirements.txt       # Python dependencies
├── .gitignore            # Git ignore rules
├── venv/                 # Virtual environment (not in git)
├── *.ipynb               # Jupyter notebooks
└── data/                 # Data files (create if needed)
```

## Recommended Workflow

1. **Start session:**
   ```bash
   cd math
   source venv/bin/activate  # Activate virtual environment
   jupyter notebook          # Start Jupyter
   ```

2. **End session:**
   - Save all notebooks
   - Clear outputs if committing to git
   - Deactivate virtual environment: `deactivate`

3. **Regular maintenance:**
   - Update dependencies: `pip install --upgrade -r requirements.txt`
   - Check for security updates: `pip list --outdated`
   - Commit changes regularly

## Additional Tools (Optional)

- **nbstripout** - Automatically strip notebook output before git commits
  ```bash
  pip install nbstripout
  nbstripout --install
  ```

- **JupyterLab** - Modern interface for Jupyter
  ```bash
  pip install jupyterlab
  jupyter lab
  ```

- **Black** - Code formatter for Python cells
  ```bash
  pip install black
  ```

## Dependencies

- NumPy - Numerical computing
- Matplotlib - Plotting and visualization
- Seaborn - Statistical data visualization
- Jupyter - Interactive notebooks
- SciPy - Scientific computing (optional)
- SymPy - Symbolic mathematics (optional)

## Tips for Learning

1. Run all cells sequentially to understand the flow
2. Experiment by modifying code cells
3. Use `Shift + Enter` to run cells
4. Try solving problems before looking at solutions
5. Create your own notebooks for practice problems

## Resources

- [NumPy Documentation](https://numpy.org/doc/)
- [Matplotlib Gallery](https://matplotlib.org/stable/gallery/index.html)
- [Jupyter Notebook Documentation](https://jupyter-notebook.readthedocs.io/)

## License

This project is for educational purposes.
