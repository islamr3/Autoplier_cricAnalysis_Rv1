# jdrf_autoplier


## Setup a virtual environment with conda
The conda package and environment manager is included in all versions of
[Anaconda](https://docs.conda.io/projects/conda/en/latest/glossary.html#anaconda-glossary),
[Miniconda](https://docs.conda.io/projects/conda/en/latest/glossary.html#miniconda-glossary),
and [Anaconda Repository](https://docs.continuum.io/anaconda-repository/).
Here we will go with the lightweight miniconda option.
Follow the links to get directions on downloading the miniconda installer for
[Windows](https://conda.io/docs/user-guide/install/windows.html),
[MacOS](https://conda.io/docs/user-guide/install/macos.html), or
[Linux](https://conda.io/docs/user-guide/install/linux.html) and run the
installer appropriate for your operating system. For example, the MacOS
directions say:
+ Open a terminal and run
```
bash Miniconda3-latest-MacOSX-x86_64.sh
```
which will open an installer screen that will walk you through installation.
+ Double check conda is updated.
```
conda update -n base conda
```
Init conda environmen with the yaml file provided
```
conda env create -f env.yaml
```

When prompted new packages will be installed, procceed by pressing `y`.
+ Activate the virtual environment
```
conda activate autoplier
```
+ Update the virtual environment (when necessary)
```
conda env update --file env.yaml --prune
```
+ To deactivate the environment, use
```
conda deactivate
```
+ To remove the environment, use
```
conda env remove -n autoplier
```
