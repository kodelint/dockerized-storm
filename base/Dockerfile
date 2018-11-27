FROM centos:centos7

MAINTAINER Satyajit Roy <satyajit@adobe.com>

RUN yum update -y && yum install java curl tar -y

RUN curl -s http://archive.apache.org/dist/storm/apache-storm-1.2.2/apache-storm-1.2.2.tar.gz | \
      tar zxf - -C /opt && \
      mv /opt/apache-storm-1.2.2 /opt/apache-storm

ADD configure.sh /
