# Model Orchestration
This section of the repo is about using a workflow management system (prefect) designed for orchestrating complex data workflows. 
Prefect provides a framewrok for building, scheduling, monitoring and debugging data workflows in python.


## Environment Dependencies and Installments
python == 3.11.4
scikit-learn == 1.3.2
mlflow == 2.9.2
scikit-learn == 1.3.2
numpy
pandas
fastparquet
flask
requests



### Create a virtual environment to efficiently manage your dependencies.
** conda create -n model-orch python==3.11.4
where 'model-orch' is the name of the conda environment

*** Activate with:
conda activate model-orch


### Installing dependencies in the requirements text file with this command
** pip install -r requirements.txt


## Running the Prefect server. (terminal command) 
** prefect server start 

### Deploying on Prefect
prefect deploy 3.4/orchestrate.py:main_flow -n taxi1 -p zoompool

### Starting the worker
prefect worker start -p zoompool




## Issues
** Didn't run works that demand the use of aws resources.