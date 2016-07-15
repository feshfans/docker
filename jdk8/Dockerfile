FROM centos
MAINTAINER feshfans <feshfans@163.com>

WORKDIR /opt

COPY jdk-8u91-x64.tar.gz /opt/

RUN tar xzf jdk-8u91-x64.tar.gz 

ENV JAVA_HOME /opt/jdk1.8.0_91
ENV PATH $JAVA_HOME/bin:$PATH

RUN rm -f /opt/jdk-8u91-x64.tar.gz  
 


