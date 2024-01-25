# Model Deployment
This section of the repo is about model deployment in various instances


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

gunicorn


Install dependencies with pipenv:
** pipenv install scikit-learn==1.3.2 flask --python=3.11.4
** pipenv install gunicorn

activate with:
** pipenv shell

## Running with gunicorn instead of flask
gunicorn --bind=0.0.0.0:9696 predict:app  (run in terminal)


## Building and Running with Docker

```bash
docker build -t ride-duration-prediction-service:v1 .
```

```bash
docker run -it --rm -p 9696:9696  ride-duration-prediction-service:v1
```


## Issues
** I don't have access to aws resources 