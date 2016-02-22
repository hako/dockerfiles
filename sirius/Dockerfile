#
# Dockerfile for sirius
# (c) hako
#

FROM gliderlabs/alpine
MAINTAINER Wesley Hill <wesley@hakobaito.co.uk>

RUN apk add --no-cache git make python python-dev py-pip gcc musl-dev libpq postgresql-dev \ 
    && pip install --upgrade pip \
    && pip install honcho

RUN addgroup -S sirius \
    && adduser -S -G sirius sirius

WORKDIR /home/sirius

RUN wget https://bitbucket.org/ariya/phantomjs/downloads/phantomjs-1.9.8-linux-x86_64.tar.bz2 \
    && tar jxf phantomjs-1.9.8-linux-x86_64.tar.bz2 && mv phantomjs-1.9.8-linux-x86_64/bin/phantomjs /usr/local/bin/phantomjs

ENV FLASK_CONFIG=heroku

RUN git clone https://github.com/genmon/sirius.git \
    && cd sirius \
    && pip install -r requirements.txt \
    && ./manage.py db upgrade

WORKDIR /home/sirius/sirius
USER sirius
EXPOSE 5000
