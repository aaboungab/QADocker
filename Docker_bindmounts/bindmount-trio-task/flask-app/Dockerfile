#Use Python Image
FROM python:3.7
# Install apt dependencies
RUN apt-get update && apt-get install -y python3-pip
# run pip dependencies
RUN pip3 install flask flask-sqlalchemy PyMySQL cryptography

COPY . . 
# Expose correct port
EXPOSE 5000
# Create an entrypoint
ENTRYPOINT ["python3","app.py"]
