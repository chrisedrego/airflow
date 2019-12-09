FROM python:3.7-slim-stretch
LABEL maintainer="chrisedrego"

# Blocks-Interactive pop-outs
ENV DEBIAN_FRONTEND noninteractive
# Setting the TERM to linux
ENV TERM linux

# Setting Airflow Information
ARG AIRFLOW_VERSION=1.10.6
ARG AIRFLOW_USER_HOME=/usr/local/airflow
ARG AIRFLOW_DEPS=""
ARG PYTHON_DEPS=""
ENV AIRFLOW_HOME=${AIRFLOW_USER_HOME}


# Installing the required packges
RUN apt-get update -yqq \
    && apt-get upgrade -yqq \
    && pip install -U pip setuptools wheel \
    && pip install apache-airflow[mysql]==${AIRFLOW_VERSION} \
    && apt-get autoremove -yqq --purge \
    && c \


