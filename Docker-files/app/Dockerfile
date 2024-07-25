FROM tomcat:9-jre11
LABEL "Project"="Vprofile"

RUN rm -rf /usr/local/tomcat/webapps/*
RUN echo "$(pwd)"
COPY /var/lib/jenkins/workspace/test_02/target/*.war /usr/local/tomcat/webapps/ROOT.war

EXPOSE 8080
CMD ["catalina.sh", "run"]
WORKDIR /usr/local/tomcat/
VOLUME /usr/local/tomcat/webapps
