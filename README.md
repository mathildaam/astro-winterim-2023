# Welcome to Winterim Astronomy!
**Instructor: Mathilda Avirett-Mackenzie**

## Setup instructions
### 1. Install Miniconda
To install `conda`, head over to their [website](https://docs.conda.io/en/latest/miniconda.html). This contains a bunch of links for installers as well as to the installation instructions. **Make sure you get the version for Python 3.9.**

### 2. Download the repo
Open the terminal and navigate to where you want to store the files for the class (`cd <path-to-directory>`). Now copy this command into the terminal and run it:
```
git clone https://github.com/mathildaam/astro-winterim-2023.git
```
If you have issues with this contact me.

### 3. Set up the `conda` environment
Copy this command into the terminal and run it:
```
conda env create -f env.yml
```

### 4. Run Jupyter
This series of commands will open a browser window with Jupyter running in it.
```
cd notebooks
conda activate winterim
jupyter notebook
```