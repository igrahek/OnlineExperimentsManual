# About

This manual uses Psiturk and custom JavaScript code for creating online experiments. 

Contributors: Ivan Grahek

Last update: 12/21/22

# Steps

## Installing Psiturk

Install Psiturk within a new conda environment. Psiturk currently runs only on Linux and MacOS. Python 3.7 currently works well with Psiturk, so we install that version in our conda environment.

### Install Anaconda or Miniconda
https://docs.anaconda.com/anaconda/install/index.html

### Create a conda environment
```
conda create -n psiturk
conda activate psiturk
conda install python=3.7
pip install psiturk
```

### Run a test experiment
After you have installed Psiturk, you can run an example experiment to make sure that it was successfully installed. You will run the psi-turk example locally (on your computer). Before starting Psiturk, make sure that you activate your newly created conda environment (see above). More details here: https://psiturk.readthedocs.io/en/latest/quickstart.html 

In your terminal navigate to the folder where you want your experiment to be.

Activate the conda environment

```
conda activate psiturk
psiturk
```

Create a folder with an example experiment (Stroop)
```
psiturk-setup-example 
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

