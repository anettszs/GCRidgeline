# Globular Cluster Ridgeline

## Purpose

This project focuses on the analysis of stellar data from globular clusters using data retrieved from the Gaia archive. There are two main jupyter notebooks:
- A data acquisition script that downloads relevant stellar parameters for a selected globular cluster.
- An analysis script that processes the data. It creates the color-magnitude diagram (CMD) of the cluster and then compresses it into a well-defined ridgeline.

## How to Download This Repository

You can download this repository in a few different ways:

### Option 1. Clone via Git (Recommended)

If you have Git installed, open a terminal and run:

```bash
git clone https://github.com/anettszs/GCRidgeline.git
```

### Option 2. Download as ZIP

1. Visit the repository in your browser: https://github.com/username/repo-name

2. Click the green Code button.

3. Select Download ZIP.

4. Unzip the downloaded file on your computer.


## Usage

### Option 1.

Open the notebooks with Jupyter or VS Code to explore the analysis.

### Option 2. 

Steps to deal with modern Linux:

1. You must create a virtual environment
python3 -m venv astroenv

2. Activate the virtual environment
source ~/astroenv/bin/activate

3. within the virtual environment, install all dependencies:

pip install -r requirements.txt

4. Establish a kernel tied to the virtual environment (in the command line at your terminal)

python -m ipykernel install --user --name=astroenv --display-name "Python (astroenv)"
Installed kernelspec astroenv in /home/mjoyce/.local/share/jupyter/kernels/astroenv

5. Launch jupyter notebook from within the venv

6. Once Jupyter notebook is launched, change the kernel within jupyter notebook:
Kernel → Change kernel → Python (astroenv)

## Contents

- `gaia_data_cleaning.ipynb`: Downloads the Gaia data for a Globular Cluster (with additional cleaning)
- `ridgeline.ipynb`: Creates a corresponding ridgeline 

## Requirements

- Python 3.x
- astropy
- astroquery
- statsmodels
- pandas
- matplotlib
- numpy

