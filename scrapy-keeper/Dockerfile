FROM python:3.7-bullseye

RUN apt-get update \
    && apt-get install -y build-essential git gcc python3-dev musl-dev g++ python3-numpy python3-mysqldb

RUN git clone https://github.com/aaronflorey/ScrapyKeeper.git /app
WORKDIR /app

RUN pip3 install . && pip3 install mysqlclient

RUN apt-get remove -y build-essential git gcc python3-dev musl-dev g++ python3-numpy  
