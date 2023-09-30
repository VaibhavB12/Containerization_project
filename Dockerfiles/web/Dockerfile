FROM nginx
LABEL "Project"="containerization"
LABEL "Author"="Vaibhav"
# Remove default configuration file of nginx
RUN rm -rf /etc/nginx/conf.d/default.conf
# Copy our nginx configuration file to default location
COPY nginvproapp.conf /etc/nginx/conf.d/vproapp.conf