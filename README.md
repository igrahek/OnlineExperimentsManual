# Online experiments manual

This manual uses Psiturk and custom JavaScript code for creating online experiments. 

Contributors: Ivan Grahek

Last update: 02/07/23

## Contents
1. [Installing Psiturk](#install)

### Installing Psiturk <a name="install"></a>

Install Psiturk within a new conda environment. Psiturk currently runs only on Linux and MacOS. Python 3.7 currently works well with Psiturk, so we install that version in our conda environment.

### Install Anaconda or Miniconda
** Make sure to install in a reasonable folder (do not install on top of all of your other files)
https://docs.anaconda.com/anaconda/install/index.html

### Create a conda environment
```
conda create -n psiturk
conda activate psiturk
conda install python=3.7
pip install cryptography==36.0.2  [solves a dependency issue on 02/07/2023]
pip install psiturk
```

### Run a test experiment
After you have installed Psiturk, you can run an example experiment to make sure that it was successfully installed. You will run the psi-turk example locally (on your computer). Before starting Psiturk, make sure that you activate your newly created conda environment (see above). More details here: https://psiturk.readthedocs.io/en/latest/quickstart.html 

In your terminal navigate to the folder where you want your experiment to be.

Activate the conda environment
```
conda activate psiturk
```

Start psiturk (Ignore the warning about the AWS credentials)
```
psiturk
```

Create a folder with an example experiment (Stroop)
```
psiturk-setup-example 
```

Go into the newly created folder
```
cd psiturk-example 
```

Run the experiment in your browser
```
psiturk server on
psiturk debug
```

To get the link to the experiment (e.g., to send to a collaborator once the experiment is running on the server). 
```
psiturk debug -p
```


