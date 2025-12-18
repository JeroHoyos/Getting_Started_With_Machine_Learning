# ML seminar

## 01 - Creating_virtual_environments ##

**Table of Contents**
<br>
This markdown shows how to create and manage virtual environments to isolate the Python version and the Packages used.

## Creating virtual a enviroment ##

First, open a terminal in the folder where you want to work, then run:

```bash
python3 -m venv .venv
```

Where `.venv` is the folder that contains the environment configuration.

You can also specify the Python version using:

```bash
python3 -m venv .venv --python=python3.10
```

## Activating the Environment

After creating the virtual environment, you need to activate it.

### On Windows

```bash
.venv\Scripts\activate
```

### On Linux / macOS

```bash
source .venv/bin/activate
```

### Deactivating the Environment

When you finish working with the virtual environment, deactivate it by running:

```bash
deactivate
```

## Packages

Once the virtual environment is active, you can install packages inside the environment.

```bash
python -m pip install numpy
```

You can also upgrade the packages using:

```bash
pip install --upgrade package_name
```

Below are some useful `pip` commands:

* Show information about a package
```bash
pip show package_name
```
* List installed packages
```bash
pip list
```
* Generate a list of installed packages
```bash
pip freeze > requirements.txt
```
* Install packages from a requirements file
```bash
python -m pip install -r requirements.txt
```
* Uninstall a package
```bash
pip Unistall package_name
```
**Well Done!** Let's move to the [next section](1-02_numpy.ipynb). 
