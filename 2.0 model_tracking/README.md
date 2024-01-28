# Model Tracking
This section of the repo is about managing the end-to-end machine learning lifecycle. 
Tasks here include experiment tracking, reproducibility, model packaging and deployment
Tool used here is MLflow


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



### Creates a conda virtual environment with the above packages
** conda create -n model-tracking-env python==3.11.4



### Pip install dependencies including mlflow
** pip install -r requirements.txt


## Running the mlflow ui/server using sqlite(terminal command) 
** mlflow ui --backend-store-uri sqlite:///mydb.sqlite
** mlflow server --backend-store-uri sqlite:///mydb.sqlite

