[![Shipping files](https://github.com/neuefische/ds-random-forest/actions/workflows/workflow-02.yml/badge.svg?branch=main&event=workflow_dispatch)](https://github.com/neuefische/ds-random-forest/actions/workflows/workflow-02.yml)

# Random Forest

In this repo we will have a look at various topics related to random forest.


### The way to success:

Please work in pairs through all the notebooks in this particular order:


1. [Random Forest Sklearn](1_Random_Forest_Codealong.ipynb)
2. [Random Forest Tutorial](2_Random_Forest_Tutorial.ipynb)
3. [Random Forest Exercise](3_Random_Forest_Exercise.ipynb)

The first notebook will show you how to implement
Random Forest with sklearn.
In the second notebook, Decision Trees and Random Forests are compared.
In the third notebook you can apply the random forest algorithm on Lending Club Data.

## Set up your Environment

Please make sure you have forked the repo and set up a new virtual environment. For this purpose you can use the following commands:

The added [requirements file](requirements.txt) contains all libraries and dependencies we need to execute the hands-on ml notebooks.

*Note: If there are errors during environment setup, try removing the versions from the failing packages in the requirements file. M1 shizzle.*

### **`macOS`** type the following commands : 


- Install the virtual environment and the required packages by following commands:

    ```BASH
    pyenv local 3.11.3
    python -m venv .venv
    source .venv/bin/activate
    pip install --upgrade pip
    pip install -r requirements.txt
    ```
### **`WindowsOS`** type the following commands :

- Install the virtual environment and the required packages by following commands.

   For `PowerShell` CLI :

    ```PowerShell
    pyenv local 3.11.3
    python -m venv .venv
    .venv\Scripts\Activate.ps1
    python -m pip install --upgrade pip
    pip install -r requirements.txt
    ```

    For `Git-bash` CLI :
  
    ```BASH
    pyenv local 3.11.3
    python -m venv .venv
    source .venv/Scripts/activate
    python -m pip install --upgrade pip
    pip install -r requirements.txt
    ```
     **`Note:`**
    If you encounter an error when trying to run `pip install --upgrade pip`, try using the following command:

    ```Bash
    python.exe -m pip install --upgrade pip
    ```
    
The data used in this notebook is saved in a `.zip` file. To unzip it, copy the block below into your terminal:

```Bash
unzip data.zip
```

