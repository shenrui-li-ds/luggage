# luggage
Frequently used commands and requirements for various projects.

1. Create conda virtual environment
    ```bash
    conda create -n env_name python=3.11
    conda activate env_name
    ```

2. Create ipykernel in Azure ML
    ```bash
    python -m ipykernel install --user --name env_name --display-name "Python (env_name)"
    pip install boto3 botocore
    ```

3. Install requirements
    ```bash
    cd <repository-directory>
    pip install pip-tools
    pip-compile requirements.in
    pip install -r requirements.txt
    ```

4. Activate conda virtual environment
    ```bash
    conda activate env_name
    ```

5. Remove conda virtual environment
    ```bash
    conda deactivate env_name
    conda remove --name env_name --all
    ```

6. Remove ipynerknel
    - Check kernel list
        ```bash
        jupyter kernelspec list
        ```
    - Remove kernel
        ```bash
        jupyter kernelspec uninstall env_name
        ```