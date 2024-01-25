FROM python:3.11.4-slim

RUN pip install -U pip
RUN pip install pipenv 


WORKDIR /app

COPY [ "Pipfile", "Pipfile.lock", "./" ]

#RUN apt-get update && apt-get install -y build-essential


RUN pipenv install --system --deploy

COPY [ "predict.py", "linReg.bin", "./" ]

EXPOSE 9696

ENTRYPOINT [ "gunicorn", "--bind=0.0.0.0:9696", "predict:app" ]