FROM jenkins:latest

USER root
RUN apt-get update -y -qq
RUN apt-get install -y -qq build-essential
RUN apt-get install -y python2.7 python-pip python-dev
RUN apt-get install -y lsof
RUN pip install virtualenv
RUN pip install tox

USER jenkins