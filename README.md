# Setup
1. Install python 3.12
1. Make sure cuda is installed. For the project, WSL on Windows is used, and Cuda SDK 12.1 was installed
1. Follow the [insturctions](https://github.com/fastai/fastsetup) to setup fastai dependencies.
1. Create a python virtual enviornment using the following command
    ```bash
    python -m venv .venv
    ```
1. Open the python environment configuration file: [./.venv/pyvenv.cfg](./.venv/pyvenv.cfg) and add the following configuration. This allows the virtual environment uses the system site packages, since every new virtual environment does not have any packages pre-installed.
    ```
    include-system-site-packages = true
    ```
1. Install and setup the jupyter notebook with the following command. (It is recommended to install notebook outside of the virtual env)
    ```bash
    pip install notebook
    ```
1. Activate virutal .venv
    ```bash
    . ./.venv/bin/activate
    # to deactivate use the command below
    . ./.venv/bin/deactivate
    ```
1. Start the Jupyter Notebook with the following command.
    ```bash
    jupyter notebook
    ```
1. After the notebook has started, you can access the URL provided in the console. e.g., http://localhost:8888/tree?token=<auto_token>
