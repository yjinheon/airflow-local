FROM apache/airflow:2.7.3-python3.11
USER root
RUN apt-get update && apt-get install -y \
    libpq-dev \
    gcc \
    python3-dev \
    vim \
    openjdk-11-jdk \
    && apt-get clean

ENV JAVA_HOME /usr/lib/jvm/java-11-openjdk-amd64

USER airflow
RUN pip install apache-airflow apache-airflow-providers-apache-spark pyspark 
