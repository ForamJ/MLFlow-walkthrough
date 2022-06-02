# Managing the end-to-end machine learning lifecycle with MLFlow

This Repository contains the resources for my tutorial **"Managing the end-to-end machine learning lifecycle with MLFlow"** at pyData/pyCon Berlin 2019.

# Basic setup

## Setup the environment
- clone this repository
- **with virtualenv (recommended)**
  - install virtualenv: `pip install virtualenv`
  - create a new environment: `virtualenv mlflow_tutorial`
  - activate the environment: `source mlflow_tutorial/bin/activate`
  - run `pip install -r requirements.txt`
  
- **with pipenv** 
  - install pipenv: `pip install pipenv`
  - run `pipenv install` in the directory of the Pipfile
  - activate the environment by `pipenv shell`

## Launch MLFlow Server
```sh
mlflow server --backend-store-uri mlruns/ --default-artifact-root mlruns/ --host 0.0.0.0 --port 5000
```
![MLFlow UI](https://user-images.githubusercontent.com/105413916/171628797-5813240b-f9ca-4bed-ac4c-0bce437520b4.png)

## The notebook
- Get the `hands_on_example.ipynb`
- run `jupyter notebook`

# Advanced setup

## Setup the environment
- install postgresql: `sudo apt-get install postgresql postgresql-contrib postgresql-server-dev-all`
