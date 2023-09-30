FROM mysql:5.7.25
LABEL "Project"="containerization"
LABEL "Author"="Vaibhav"
# set envioronment variables to access mysql when container is created
ENV MYSQL_ROOT_PASSWORD="vprodbpass"
ENV MYSQL_DATABASE="accounts"
# we can copy & download files from URL with ADD but COPY only copy local files 
# db_backup.sql contains database commands & we are pushing it to /docker-entrypoint-initdb.d 
# /docker-entrypoint-initdb.d used with database Docker images & allows you to automatically execute SQL scripts
ADD db_backip.sql