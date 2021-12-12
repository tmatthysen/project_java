FROM tomcat:latest
WORKDIR /usr/local/tomcat/webapps
ADD target/maven-0.0.1-SNAPSHOT.war .
RUN sed -i 's/port="8080"/port="8081"/' /usr/local/tomcat/conf/server.xml
EXPOSE 8081
CMD ["catalina.sh","run"]