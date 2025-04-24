# Use the official Apache Airflow image as the base image
FROM apache/airflow:2.10.5

# Switch to root user to install system dependencies
USER root
RUN mkdir -p /app/models

COPY requirements.txt /tmp/rquirements.txt
RUN pip install  -p/tmp/models\requirements.txt
# Switch back to the airflow user for security
USER airflow

