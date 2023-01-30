FROM ubuntu:latest

WORKDIR /app

COPY . /app

RUN apt-get update \
    && apt-get install nano \
    && apt-get install vim \
    && Y \
    && apt-get install pip \
    && pip install Django \
    && pip install Django-upgrade \
    && apt-get upgrade python3 \
    && python3 -m django --version 

# COPY . /app    



# FROM python:3.8.1-alpine

# WORKDIR /src

# ENV PYTHONDONTWRITEBYTECODE 1
# ENV PYTHONUNBUFFERED 1

# COPY ./requirements.txt /src/requirements.txt

# RUN set -eux \
#     && apk add --no-cache --virtual .build-deps build-base \
#     libressl-dev libffi-dev gcc musl-dev python3-dev \
#     postgresql-dev \
#     && pip install --upgrade pip setuptools wheel \
#     && pip install -r /src/requirements.txt \
#     && rm -rf /root/.cache/pip

# COPY . /src/