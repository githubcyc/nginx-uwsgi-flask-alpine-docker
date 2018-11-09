FROM python:3.6.6-alpine

# https://github.com/docker-library/python/blob/master/3.6/alpine3.6/Dockerfile
# https://stackoverflow.com/questions/38568476/installing-seaborn-on-docker-alpine

COPY repositories.txt /etc/apk/repositories
COPY pip.conf /etc/pip.conf
COPY requirements.txt /app/

WORKDIR /app

# Install dependencies and package it
RUN apk add --no-cache --virtual .build-deps \
    g++ && \
    ln -s /usr/include/locale.h /usr/include/xlocale.h && \
    pip install -r requirements.txt && \
    # removing package installed
    apk del .build-deps

CMD tail -f /dev/null