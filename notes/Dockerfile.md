```
FROM centos:latest
RUN yum -y install httpd  
RUN  systemctl enable httpd.service 
EXPOSE 80

COPY jdk1.8 /usr/local/jdk1.8.0_121
ENV JAVA_HOME=/usr/local/jdk1.8.0_121
ENV PATH $JAVA_HOME/bin:$PATH
ENV CLASSPATH .:$JAVA_HOME/lib/dt.jar:$JAVA_HOME/lib/tools.jar

CMD /usr/sbin/init
```
