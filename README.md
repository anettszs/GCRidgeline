# Globular Cluster Ridgeline

## Function
We present a new method and a corresponding code to compress the color magnitude diagram of a globular cluster into a representative curve, called a ridgeline, that can be more readily compared to isochrone models, among other applications. This compression method preserves the physical properties of the cluster, including the morphology of the CMD.

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

### Option 1. Jupyter or VS Code 

Open the notebooks with Jupyter or VS Code to explore the analysis. (Or try Google Colab)

### Option 2. Virtual environment

Steps to deal with modern Linux:

1. You must create a virtual environment

```bash
python3 -m venv astroenv
```

2. Activate the virtual environment
source ~/astroenv/bin/activate

3. within the virtual environment, install all dependencies:

```bash
pip install -r requirements.txt
```

4. Establish a kernel tied to the virtual environment (in the command line at your terminal)

python -m ipykernel install --user --name=astroenv --display-name "Python (astroenv)"
Installed kernelspec astroenv in /home/mjoyce/.local/share/jupyter/kernels/astroenv

5. Launch jupyter notebook from within the venv

6. Once Jupyter notebook is launched, change the kernel within jupyter notebook:
Kernel → Change kernel → Python (astroenv)

### Option 3. Conda virtualenv version

Using a conda virtual environment

This part assumes that you have a version of Anaconda installed. We recommend the Miniconda distribution for the purposes of this package: https://www.anaconda.com/docs/getting-started/miniconda/install 

1. First we create a conda virtual environment (you can replace 'astroenv' with the name of your choice):

```bash
conda create --name astroenv
```

If you want to specify python versions and other parameters here, consult the conda pages: https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html

2. Activate the environment: 

```bash
conda activate astroenv
```

3. And install the requirements in this new environment. 

4. Establish a kernel tied to the virtual environment for Jupyter to recognize: 

```bash
python -m ipykernel install --user --name=astroenv --display-name "Python (astroenv)"
```

5. Open the notebooks in Jupyter notebook/lab and switch to the new kernel.


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

## License

This project is licensed under the MIT License.

## Acknowledge

Special thanks to my mentors: [@mjoyceGR](https://github.com/mjoyceGR), [@lacalaca85](https://github.com/lacalaca85), [@cskalup](https://github.com/cskalup)   
This research was supported by the ‘SeismoLab’ KKP-137523 grant and the TKP2021-NKTA-64 excellence grant
of the Hungarian Research, Development and Innovation Office (NKFIH). A. S-Zs. acknowledges the undergraduate
research assistant program of Konkoly Observatory.