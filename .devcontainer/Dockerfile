FROM mcr.microsoft.com/devcontainers/python:3.9

# Install Airflow and ClickHouse dependencies manually
RUN pip install "apache-airflow==2.7.1" \
    "apache-airflow-providers-common-sql" \
    "airflow-clickhouse-plugin" \
    "clickhouse-driver" \
    "pandas"

# Set environment variables
ENV AIRFLOW_HOME=/opt/airflow
ENV AIRFLOW__CORE__LOAD_EXAMPLES=false

WORKDIR ${AIRFLOW_HOME}
