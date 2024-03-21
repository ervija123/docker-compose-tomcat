# Dockerfile for TOMCAT
FROM tomcat:8.5.60-jdk8-openjdk-buster

# Usual maintenance
RUN rm -rf /usr/local/tomcat/webapps/*

# Create Dirs
RUN mkdir /usr/local/tomcat/ssl

# set TOMCAT config (support for SSL)
COPY server.xml /usr/local/tomcat/conf/

CMD ["catalina.sh", "run"]
