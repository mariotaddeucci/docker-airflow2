ARG PYTHON_V=3.7
FROM python:$PYTHON_V

ENV AIRFLOW_HOME=/
ENV AIRFLOW__CORE__LOAD_EXAMPLES=False
ARG AIRFLOW_VERSION=2.1.2
ENV AIRFLOW_VERSION=${AIRFLOW_VERSION}

WORKDIR ${AIRFLOW_HOME}

COPY ./script/ .
RUN . ./setup.sh

CMD ["python", "start.py"]
