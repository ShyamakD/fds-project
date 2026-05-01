# FDS Project

## Overview

This is a Foundations of Data Science project with a clean structure for experimentation, modeling, and collaboration.

---

## Setup (First Time)

### 1. Clone the repository

```bash
git clone <repo-url>
cd fds-project
```

### 2. Install Conda (if not installed)

Install Miniconda or Mambaforge, then restart your terminal.

Check installation:

```bash
conda --version
```

---

### 3. Create environment

```bash
conda env create -f environment.yml
conda activate fds-project
```

---

### 4. Register Jupyter kernel

```bash
python -m ipykernel install --user --name=fds-project --display-name "Python (fds-project)"
```

---

## Running the Project

### Start Jupyter

```bash
    jupyter notebook
```

Select kernel:

```
Python (fds-project)
```

---

## Project Structure

```
notebooks/      → experiments and analysis
src/            → reusable code
data/           → local data (not pushed)
reports/        → generated outputs
```

---

## Data

Place datasets inside:

```
data/raw/
```

Do not commit large data files to GitHub.

---

## Adding Dependencies

If you install new packages:

```bash
conda install <package>
```

Then update environment file:

```bash
conda env export > environment.yml
```

---

## Notes

- Keep reusable logic inside `src/`, not notebooks
- Keep notebooks clean (restart & clear outputs before pushing)
- Always activate environment before working

---

## Quick Start (for collaborators)

```bash
git clone <repo-url>
cd fds-project
conda env create -f environment.yml
conda activate fds-project
jupyter notebook
```

# fds-project
