#OS version, core
FROM ubuntu:20.04
#Update and upgrade
RUN apt-get update -y && apt-get upgrade -y
#Python and pip install
RUN apt-get install python3 python3-pip -y
#Flask install
RUN pip3 install flask
#Copy to opt
COPY app.py /opt/app.py
#Entrypoint to start
ENTRYPOINT FLASK_APP=/opt/app.py flask run --host=0.0.0.0 --port=5000
