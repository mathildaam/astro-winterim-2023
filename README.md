# Welcome to Winterim Astronomy!
**Instructor: Mathilda Avirett-Mackenzie**

## Setup instructions
### 1. Install Miniconda
To install `conda`, head over to their [website](https://docs.conda.io/en/latest/miniconda.html). This contains a bunch of links for installers as well as to the installation instructions.

#### For Windows
1. Scroll to the installer for **Python 3.9** for Windows, and click the link to download the file.
2. Once downloaded, click on the executable to run it.
3. Follow the installation prompts. The recommended settings should be fine, but don't hesitate to ask if you're unsure.

#### For Mac
1. Scroll to the installer for **Python 3.9** for Mac OS, and click the link to download the file.
2. Open the Terminal program.
3. Type `cd ~/Downloads`
and press enter. This runs the command to enter your Downloads folder.  
4. Type `bash Mini` and press tab, followed by enter. This will start the installer.  
5. Follow the installation prompts. The recommended settings should be fine, but don't hesitate to ask if you're unsure.

### 2. Download this repo

#### Via git (recommended method for Mac)
In the terminal, run the following commands:
```
cd ~
git clone https://github.com/mathildaam/astro-winterim-2023.git
```

#### Via zip (works for Windows or Mac)
1. Click the green "Code" button and from the dropdown menu, click "Download ZIP"
2. Extract the zip file when downloaded. I recommend putting it in a directory called `astro-winterim-2023` in your home directory.

### 3. Set up the `conda` environment
In the terminal (Mac) or Anaconda prompt (Windows), run the following.
```
cd ~/Downloads/astro-winterim-2023
conda env create -f env.yml
```

## Running Jupyter
In the terminal (Mac) or Anaconda prompt (Windows), run the following.
```
cd ~/Downloads/astro-winterim-2023/notebooks
conda activate winterim
jupyter notebook
```

