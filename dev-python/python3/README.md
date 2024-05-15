# Development environments for wps application

## Start using

Work in the virtual environments

To create a virtual environment, go to your project’s directory and run the following command. This will create a new virtual environment in a local folder named .venv:

``` bash
python3 -m venv .venv
```

Before you can start installing or using packages in your virtual environment you’ll need to activate it. Activating a virtual environment will put the virtual environment-specific python and pip executables into your shell’s PATH.

``` bash
source .venv/bin/activate
```

To confirm the virtual environment is activated, check the location of your Python interpreter:

``` bash
which python
```

While the virtual environment is active, the above command will output a filepath that includes the .venv directory, by ending with the following:

``` bash
.venv/bin/python
```

 >See also Python Packaging User Guide: [Creating and using virtual environments](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#create-and-use-virtual-environments)
