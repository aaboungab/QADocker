# Derived from official mysql image (our base image)
FROM mysql:5.7
ENV MYSQL_ROOT_PASSWORD=123
# Add a database
ENV MYSQL_DATABASE flaskapp-db
# Add the content of the .sql file to your image
COPY ./CreateTable.sql/ /docker-entrypoint-initdb.d/
# All scripts in docker-entrypoint-initdb.d/ are automatically
# executed during container startup
