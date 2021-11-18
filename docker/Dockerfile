FROM python:3.7

RUN apt update && \
    apt install -y vim git curl

RUN pip install --upgrade pip
ADD ./docker/requirements.txt /tmp/requirements.txt
RUN pip install -r /tmp/requirements.txt

#Install azure cli

RUN curl -sL https://aka.ms/InstallAzureCLIDeb | bash
