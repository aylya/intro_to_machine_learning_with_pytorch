# Installations

You are required to download and install the following free softwares for this workshop.

- [Anaconda Package Manager](https://www.anaconda.com/)
- [Visual Studio Code](https://code.visualstudio.com/)
- [Git Version Control System](https://git-scm.com/)


## Setting up your conda environment from environment.yml


```
conda env create -f environment.yml

```

## Activate


```
conda activate pytorch
```


## Setting up your conda environment step by step

When you download and install Anaconda, you are also installing the latest version of Python, Jupyter Notebooks and several useful data science libarries which are essential for data manipulation and developing machine learning applications.

Main benefit of using Anaconda is having the ability to setup up your own development environment. Often you will need to work with a specific version of Python and associated packages depending on the project requirements.  Having the ability to create new environments and switching between them helps you avoid unnecessary errors. In addition, it enables you to run other people's code or publish your own.

To create a new environment, start the `Anaconda Prompt` and execute the following code to create your own  environment.


```conda
conda create -n pytorch python=3.7

Solving environment: done
## Package Plan ##

  environment location: C:\Users\Username\Anaconda3\envs\my_env

Proceed ([y]/n)? y
```

## Testing your environment

You can test that you have successfully created a new environment by activating it using:

```conda
conda activate pytorch

(my_env) C:\Users\Username>
```

Then, you can check what packages have been already installed within your environment using:

```conda
conda list pytorch

# packages in environment at C:\Users\Username\Anaconda3\envs\my_env:
#
# Name                    Version                   Build  Channel
attrs                     19.1.0                   py37_1
backcall                  0.1.0                    py37_0
ca-certificates           2019.1.23                     0
...                        ...                        ...
webencodings              0.5.1                    py37_1
wheel                     0.33.1                   py37_0
wincertstore              0.2                      py37_0
zlib                      1.2.11               h62dcd97_3
```

```conda
(my_env) C:\Users\Username>
```

Once you environment is set, and you have it activated, simply run the following commands to install all the required packages for this workshop.


#### Installing Numpy

```conda
conda install numpy
```

#### Installing Matplotlib

```conda
conda install matplotlib
```

#### Installing Pytorch - WINDOWS

```conda
conda install pytorch-cpu torchvision-cpu -c pytorch
```

#### Installing Pytorch - MacOS

To install pytorch for MacOS you will need to run the following command instead:

```
conda install pytorch torchvision -c pytorch
```

#### Test Pytorch Installation

Check one last time that you have everything installed and ready to go using:

```conda
conda list
```

You can also try importing `torch` and `torchvision` packages. If you don't get any errors, you're good to go.

## Installing Jupyter Notebooks

Open the `Anaconda Navigator` then select your newly created environment `my_env` from the top drop down menu on the main page, then press the `install` button underneath the Jupyter Notebooks card. When installed, press the `launch` button to start the Jupyter notebooks on your browser. Simply navigate to the notebook files we have provided in this repo to open the notebook.

```
conda install -c conda-forge jupyterlab

```
## Starting VS Code via Anaconda Navigator

To ensure your VS code is configured to your environment `my_env`, simply launch VS Code via `Anaconda Navigator` while having your environment selected from the drop down menu.

## Learn More

- [Setting up conda environments](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#viewing-a-list-of-your-environments)
- [Codecademy - How to work with Jupyter notebooks - 11 min watch](https://www.codecademy.com/articles/how-to-use-jupyter-notebooks)
