# Jupyter Lab Study Notes

## Installation

### Install miniconda on both server and local sides.

* Installing on Linux: https://docs.conda.io/projects/conda/en/latest/user-guide/install/linux.html#
* Installing on MacOS: https://docs.conda.io/projects/conda/en/latest/user-guide/install/macos.html

### Install Jupyter Lab through conda.


## Running

### Running server side locally.

1. Server side login: ```ssh -l mx31 stampede2.tacc.utexas.edu```
2. Switch to computing mode: ```idev -p normal -N 1 -m 300```
3. Server side command: ```jupyter-lab  --no-browser --port=8787  --ip=0.0.0.0 ```
4. Local side command: ```ssh -N -L 8787:c455-044:8787 mx31@stampede2.tacc.utexas.edu``` 
   * c455-044 should be replaced by the proper computing node index.
5. Open the link in the browser: http://localhost:8787/lab
6. Fill in the block with the given token.


## Extensions

### Prerequisite: Node.js

* https://jupyterlab.readthedocs.io/en/stable/user/extensions.html
* In order to install JupyterLab extensions, you need to have Node.js installed:
```conda install -c conda-forge nodejs```

### Variable Inspector

* https://github.com/lckr/jupyterlab-variableInspector
* Command to run: ```jupyter labextension install @lckr/jupyterlab_variableinspector ```






