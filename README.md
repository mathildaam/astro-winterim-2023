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
cd ~/Downloads/
git clone https://github.com/mathildaam/astro-winterim-2023.git
```

#### Via zip (works for Windows or Mac)
1. Click the green "Code" button and from the dropdown menu, click "Download ZIP"
2. Extract the zip file when downloaded. I recommend putting it in a directory called `astro-winterim-2023` in your home directory.

### 3. Set up the `conda` environment
In the terminal (Mac) or Anaconda prompt (Windows), run the following.
```
cd ~/Downloads/astro-winterim-2023-master
conda env create -f env.yml
```

## How to use the terminal
The terminal is a tool for viewing the files in your computer, like Finder in Mac and File Explorer$^{\ast}$ in Windows. The terminal is a much older and simpler program, running only with text inputs and outputs. But, once you get used to it, it's powerful and very simple to use.

$^{\ast}$_Note: for this exercise, we're using the Anaconda Prompt in Windows rather than File Explorer._

When you open the terminal, you start out in your home directory. This is where your computer keeps its standard directories like Documents, Downloads, Pictures, etc. All the directories on your computer can be thought of as being boxes nested inside each other. Documents, Downloads, and Pictures are nested in your home directory. When you click download on the zip file of this repository, it ends up in a directory nested in your Downloads directory.

This structure is represented by addresses, such as
```
~/Downloads/astro-winterim-2023-master/
```
(`~` is a special character representing home)

Basic commands for navigating the terminal:
* `ls` (Mac/Linux) or `dir` (Windows): print all the files in the directory you're currently in
* `cd`: change directory. You follow this command with the address of the directory you want to move to. Moving up a directory can be accomplished by `cd ..`

A very useful feature of the terminal is its autocomplete. If you type the first few letters of an address and press the `tab` key, it'll automatically complete the address if it exists, and if there's multiple possibilities it'll list them (press `tab` a few times). 

## Running Jupyter
We'll do coding examples in Jupyter, which is a useful interface for combining code with text commentary. It's also an easy way to run code in manageable pieces to test it as you're writing it.

To start up Jupyter, run the following commands in the terminal (Mac/Linux) or Anaconda Prompt (Windows).
1. Move into the code directory. 
```
cd ~/Downloads/astro-winterim-2023-master/notebooks
```
If pasting this command doesn't work, you may have to do a bit of sleuthing to find the files. You can use `cd` to move one directory at a time and `ls` to see if the directory or file you're looking for exists.
2. Start up conda.
```
conda activate winterim
```
This tells Python where to look for the packages we have installed to help us with our code.
3. Start running Jupyter.
```
jupyter notebook
```
This will open a browser window or tab running the Jupyter program.

## Adding packages to `conda`
Sometimes we realize we need to use a package that we didn't install when we set up the `conda` environment. Fortunately, `conda` makes this really easy:
```
conda install <name-of-package> -n winterim
```
Where the command says `<name-of-package>`, you'll need to insert the name of the package you need to use. 