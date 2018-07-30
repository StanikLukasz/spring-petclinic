FROM centos/systemd

RUN yum -y install wget
RUN wget -O /etc/yum.repos.d/jenkins.repo https://pkg.jenkins.io/redhat/jenkins.repo
RUN rpm --import https://pkg.jenkins.io/redhat/jenkins.io.key
RUN yum -y install jenkins
RUN yum -y install java-1.8.0-openjdk
RUN systemctl enable jenkins

EXPOSE 8080

CMD ["/sbin/init"]
