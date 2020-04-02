#Use Python Image
FROM python:3.5
# Install apt dependencies
RUN apt-get update
RUN apt install -y python3
RUN apt install -y python3-pip
# Copy contents into image
COPY . .
# run pip dependencies
RUN pip3 install flask
RUN pip3 install flask-sqlalchemy
RUN pip3 install PyMySQL
#define variables to be obtained from local terminal session
# Expose correct port
EXPOSE 5000
# Create an entrypoint
ENTRYPOINT ["/usr/local/bin/python", "app.py"]
