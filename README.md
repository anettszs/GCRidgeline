# Globular Cluster Ridgeline

This project focuses on the analysis of stellar data from globular clusters using data retrieved from the Gaia archive. There are two main jupyter notebooks.

\begint{itemize}
\item A data acquisition script that downloads relevant stellar parameters for a selected globular cluster.
\item An analysis script that processes the data. It creates the color-magnitude diagram (CMD) of the cluster and then compresses it into a well-defined ridgeline.
\end{itemize}

## Contents

- `gaia_data_cleaning.ipynb`: Downloads the Gaia data for a Globular Cluster (with additional cleaning)
- `ridgeline.ipynb`: Creates a corresponding ridgeline 

## Requirements

- Python 3.x
- astropy
- statsmodels
- pandas
- matplotlib
- numpy

## Usage

Open the notebooks with Jupyter or VS Code to explore the analysis.
