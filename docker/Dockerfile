FROM puckel/docker-airflow:1.10.8
USER root

# .............
# EXTRA STUFFS
# .............
COPY docker/entrypoint.sh /entrypoint.sh
RUN rm $AIRFLOW_HOME/airflow.cfg

COPY requirements-airflow.txt requirements.txt
RUN pip3 install -r requirements.txt

# .............
# EXTRA STUFFS
# .............
USER airflow
