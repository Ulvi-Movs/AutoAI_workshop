# Pre-installation setup

## Terminal settings for M-chips users

We need to open use Rosetta to emulate the Intel architecture. What should be noticed is that also tensorflow should be
installed using conda.

You need to change terminal setting:

Navigate to Applications -> Utilities -> Terminal, then right-click and choose "Get Info", and check "Open using Rosetta".
Close previously opened Terminal window (if you had any) and open a new one.

Create python environment
---
## For not M-chips users
```bash
conda create -n workshop_env python=3.10
conda activate workshop_env
```
---
## For M-chips users
Make sure you are running the terminal as Rosetta. Then type:
```bash
CONDA_SUBDIR=osx-64 conda create -n workshop_env python=3.10
conda activate workshop_env
conda config --env --set subdir osx-64
```
---
## Install requirements
Type in terminal:
```bash
pip install -r requirements.txt 
```
---
## Run jupyter server
Type in terminal:
```bash
jupyter notebook
```
then choose notebook that you want to run and start your journey.