#FROM python:3.9-alpine3.12
FROM python:3.7-alpine
MAINTAINER raeswar2.

ENV PYTHONUNBUFFERED 1

# Install dependencies
COPY  ./requirements.txt /requirements.txt
RUN pip install -r /requirements.txt

# Setup directory structure
RUN mkdir /app
WORKDIR /app
COPY . /app

RUN adduser -D user
USER user

