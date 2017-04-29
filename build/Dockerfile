FROM centos:7.3.1611

ARG SPARK_URI=https://archive.apache.org/dist/spark/spark-2.1.0/spark-2.1.0-bin-hadoop2.7.tgz

RUN yum -y update
RUN yum -y install java-1.8.0-openjdk

WORKDIR /tmp
RUN curl -O $SPARK_URI

WORKDIR /opt
RUN tar -xf /tmp/spark-2.1.0-bin-hadoop2.7.tgz

WORKDIR ./spark-2.1.0-bin-hadoop2.7/bin
