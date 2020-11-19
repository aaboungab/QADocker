# Use Python Image
FROM python:3.7
# Install apt dependencies
RUN apt-get update && apt-get install -y python3-pip
# Copy contents into image
COPY . .
# Run pip dependencies
RUN pip3 install Flask
# Expose the correct port
EXPOSE 5000
# Create an entrypoint
ENTRYPOINT ["python3", "app.py"]
