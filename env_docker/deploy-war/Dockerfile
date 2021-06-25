FROM tomcat:9
MAINTAINER khaledinat <khaledinat@gmail.com>

#Delete existing ROOT folder

RUN rm -rf /usr/local/tomcat/webapps/ROOT

#Copy war to tomcat path
COPY ROOT.war /usr/local/tomcat/webapps/