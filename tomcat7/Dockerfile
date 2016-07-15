FROM feshfans/jdk:8u91
MAINTAINER feshfans <feshfans@163.com>

WORKDIR /opt/
COPY tomcat-8.0.36.tar.gz /opt/

RUN tar xzf tomcat-8.0.36.tar.gz

RUN rm -f tomcat-8.0.36.tar.gz
ENV CATALINA_BASE /opt/apache-tomcat-8.0.36
ENV CATALINA_PID /var/run/tomcat.pid
ENV CATALINA_SH /opt/apache-tomcat-8.0.36/bin/catalina.sh

VOLUME ["/opt/apache-tomcat-8.0.36/webapps/"]

EXPOSE 8080 9090

ENTRYPOINT ["/opt/apache-tomcat-8.0.36/bin/catalina.sh","run"]
