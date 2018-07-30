FROM centos:7

RUN yum -y install git
RUN yum -y install maven
RUN yum -y install java-1.8.0-openjdk

ENV JAVA_HOME /usr/lib/jvm/java-1.8.0-openjdk

EXPOSE 8080

RUN git clone https://github.com/StanikLukasz/spring-petclinic; cd spring-petclinic; ./mvnw install

CMD  cd spring-petclinic; git pull https://github.com/StanikLukasz/spring-petclinic; ./mvnw spring-boot:run


