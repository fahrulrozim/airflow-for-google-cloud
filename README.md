# airflow-for-google-cloud

This is a python script for Apache Airflow DAG files using xcoms integrated with uploading to Google Cloud Storage.

Pre-requisite:
1. Google cloud credentials : `google_credentials.json`.
    Store it in `$HOME` directory with command:
    `cd ~ && mkdir -p ~/.google/credentials/`
    `mv <path/to/your/credentials>.json ~/.google/credentials/google_credentials.json`
2. Python >= 3.7
3. Docker

Here is how to run airflow:
1. Create directory `dags`, `logs` and `plugins`. In this repo, you just need to make `logs` and `plugins` since `dags` is already filled with my python script.
2. Run `docker-compose up`
3. You can see the airflow in webserver through `localhost:8080` in your browser.
4. Login through with username `airflow` and password `airflow`.
5. Choose your dags files to run.
