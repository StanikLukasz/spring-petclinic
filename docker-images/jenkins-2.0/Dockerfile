FROM jenkins/jenkins:lts

USER root

RUN apt-get install git

#RUN \
#git init; \
#git remote add origin https://github.com/StanikLukasz/Jenkins-backup; \
#git fetch --all; \
#git reset --hard origin/master 

RUN git clone https://github.com/StanikLukasz/Jenkins-backup.git

ENV JENKINS_HOME "/Jenkins-backup"

RUN mkdir /Jenkins-backup/.ssh; \
ssh-keygen -f /Jenkins-backup/.ssh/id_rsa -N ""

