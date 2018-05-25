
[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/caseygrun/kazlab-python-workshop/master)


Please follow these instructions to install Python and the required dependencies.

## If you ALREADY HAVE a Python installation that you would like to keep:

### macOS:
+ You will create a "Virtual Environment" to work for this workshop. This will keep the Python packages you install today separate from your global Python packages or other environments you may want to use

1. Open a Terminal. Change to the directory where you're reading this file. For example, if you downloaded to `~/Downloads/2018-05-25_Python_workshop`, enter:

        cd ~/Downloads/2018-05-25_Python_workshop

2. Create a virtual environment:

        python3 -m venv kaz_lab_workshop

3. "Activate" the virtual environment:

        source kaz_lab_workshop/bin/activate

    The terminal prompt should now start with `(kaz_lab_workshop)`, to remind you that you're in the virtual environment.

4. Install dependencies:

        pip install -r requirements.txt

5. Start the notebook

        jupyter notebook


In the future, each time you want to start the notebook:

1. Open a Terminal; change to this directory
2. Run `activate kaz_lab_workshop`
3. Run `jupyter notebook` to start the notebook

## If you DO NOT HAVE Python

### macOS:
    
0. Make sure you do not have `conda` installed already. Open a Terminal and type 

        conda --version

    If you get `-bash: conda: command not found`, proceed. If you get `conda 4.5.1` or something similar, run

        conda update conda

    then skip to step 2. 

1. Install miniconda: 

       + Go to <https://conda.io/miniconda.html> and download the **Python 3.6** 64-bit (bash installer) under Mac OS X
       + Open a Terminal, and change to the directory where you downloaded the installer (usually `~/Downloads`)

            cd ~/Downloads 

       + Run the installer:

            sh Miniconda3-latest-MacOSX-x86_64.sh

       + Agree to the license, agree to install miniconda, and once it's installed, agree to add conda to your PATH

2. Create an environment and install dependencies:

        conda env create -f ./environment.yml 

3. Activate the environment 
        
        conda activate kaz_lab_workshop

    The terminal prompt should now start with `(kaz_lab_workshop)`, to remind you that you're in the virtual environment.
        
4. Start the notebook
    
        jupyter notebook

In the future, each time you want to start the notebook:

1. Open a Terminal; change to this directory
2. Run `conda activate kaz_lab_workshop`
3. Run `jupyter notebook` to start the notebook

### Windows:

1. Install Miniconda
    
    - Go to <https://conda.io/miniconda.html>. Download the Python **3.6** 64-bit (exe installer) under "Windows"
    - Run the installer program, agree to the license terms, and install. Leave the default options checked with respect to changing your PATH. 

2. Open an Anaconda prompt from Start menu: click the Windows icon and start type "Anaconda prompt," then click to start. A black and white terminal window should open.
3. Change to the folder where you are reading this file, using `CD`. For instance, if you downloaded this folder to `Downloads\2018-05-25_Python_workshop`, then type:
    
        cd Downloads\2018-05-25_Python_workshop

4. Create an environment and install dependencies:

        conda env create -f ./environment.yml 

5. Activate the environment 
        
        conda activate kaz_lab_workshop

6. Start the notebook
    
        jupyter notebook


In the future, each time you want to start the notebook:

1. Open a Terminal; change to this directory
2. Run `conda activate kaz_lab_workshop`
3. Run `jupyter notebook` to start the notebook