FROM python:3.7

ENV PYTHONUNBUFFERED 1

COPY ./requirements.txt /requirements.txt
RUN pip install -r /requirements.txt

RUN mkdir /wms
WORKDIR /wms
COPY ./wms /wms

RUN adduser --disabled-login user
USER user
