# PCA–GMM identification of recrystallized grains from EBSD data

This repository contains a Jupyter Notebook designed to perform PCA–GMM analysis on EBSD grain data in order to identify recrystallized and deformed grain populations.

## Repository Content

- PCA_GMM_ReX.ipynb — The main Jupyter Notebook performing data processing, Principal Component Analysis (PCA), and Gaussian Mixture Model (GMM) clustering.
- requirements.txt — List of Python dependencies automatically installed by Binder. 
- the three EBSD data files:
    - Data_1.xlsx
    - Data_2.xlsx
    - Data_3.xlsx
Each Excel file includes data of two main microstructural descriptors for each grain:
- GOS — Grain Orientation Spread
- GMKAM — Grain Median Kernel Average Misorientation

These descriptors are used to quantify the intragranular misorientation and identify recrystallized grains.

## Run the Notebook Online

The code can be run directly online without installation by using Binder, which is accessible via the button below.

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/h-latuner/PCA_GMM_ReX/HEAD?urlpath=%2Fdoc%2Ftree%2FPCA_GMM_ReX.ipynb)

Once launched, Binder will:
- Automatically install all dependencies listed in requirements.txt.
- Open the Jupyter notebook PCA_GMM_ReX.ipynb.
- Allow you to execute each cell interactively in your browser.

## Local use of the code

If you prefer to run the notebook on your own computer instead of using Binder, follow these steps:

- Download or clone this repository so that all files (PCA_GMM_ReX.ipynb, requirements.txt, and the Excel data files) are located in the same folder on your computer.
- Open a terminal (or command prompt) in that folder.

- Create and activate a virtual environment:
```bash
python -m venv .venv
source .venv/bin/activate   # On macOS/Linux
.venv\Scripts\activate      # On Windows
```

- Install the required Python libraries:
```bash
pip install -r requirements.txt
```

- Once the virtual environment has been created in the folder containing the files, you can run the Jupyter code on your usual IDE (or copy the code to use it with Python).
