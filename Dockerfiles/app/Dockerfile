# import image
FROM tomcat:8-jre11
LABEL "Project"="containerization"
LABEL "Author"="Vaibhav"
# remove default application of tomcat 
RUN rm -rf /usr/local/tomcat/webapps/*  
# Copy artifact to /usr/local/tomcat/webapps/ with ROOT.war name
COPY target/vprofile-v2.war /usr/local/tomcat/webapps/ROOT.war
# Expose container to port 8080
EXPOSE 8080 
# catalina.sh contains script to start tomcat & catalina.sh is already present in tomcat image
CMD ["catalina.sh", "run"]
# Any command we run will be executed from below path
WORKDIR /usr/local/tomcat/
# attach a volume so we can access container files to host VM
VOLUME /usr/local/tomcat/webapps/