# Environment setup for SLML coursework

Install miniconda from the offical website using python 3.7: 
https://docs.conda.io/en/latest/miniconda.html

In you terminal make sure conda works (may depend on the platform).

Windows users: Open an Anaconda Command Prompt. You should be able to see something like the following: `(base) C:\>`

Linux and MacOS users: Open a new terminal. You should be able to see something like the following: `(base) user@pc:~$`
                    
Next, we will create a conda environment, activate, and install the necessary packages. Execute the commands below one at a time:
```
conda create -n slml python=3.7
conda activate slml
conda install numpy pandas matplotlib nodejs jupyterlab ipywidgets ffmpeg -c conda-forge
conda install scikit-learn seaborn scipy -c anaconda 
conda install pytorch torchvision -c pytorch
```

Then, move to the folder with exercises and open the jupyter notebook:
```
jupyter lab
```

Your browser should open with a Jupyter Lab UI (if not, you can use URL provided by console output).

Open test.ipynb and make sure that every cell can be executed.

