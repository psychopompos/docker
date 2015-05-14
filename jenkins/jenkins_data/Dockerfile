FROM ubuntu:latest

USER root
RUN apt-get update -y -qq
RUN apt-get install -y -qq build-essential
RUN apt-get install -y python2.7 python-pip python-dev
RUN apt-get install -y lsof
RUN pip install virtualenv
RUN pip install tox

COPY default_jenkins_data /var/jenkins_home
RUN adduser jenkins
RUN chown -R jenkins /var/jenkins_home

VOLUME /var/jenkins_home

USER jenkins



