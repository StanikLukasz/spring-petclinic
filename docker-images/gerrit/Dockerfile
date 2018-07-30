FROM centos:7

RUN yum -y install java-1.8.0-openjdk-devel
RUN yum -y install python
RUN yum -y install git
RUN cd /opt; yum -y install wget; wget https://gerrit-releases.storage.googleapis.com/gerrit-2.14.4.war

EXPOSE 8080 29418

CMD cd /opt; java -jar gerrit*.war init -d gerrit_testsite
