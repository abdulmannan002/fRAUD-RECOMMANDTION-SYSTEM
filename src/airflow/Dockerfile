FROM python:3.9-slim
RUN apt-get update && apt-get install -y \
    gcc \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*
RUN pip install --no-cache-dir \
    mlflow==2.11.3 \
    psycopg2-binary==2.9.9 \
    boto3==1.34.88
WORKDIR /app
RUN useradd -m mlflow
USER mlflow