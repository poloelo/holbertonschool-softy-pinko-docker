FROM ubuntu:latest

WORKDIR /app

COPY . /app

RUN apt-get update && apt-get upgrade -y
RUN apt-get install python3 -y
RUN apt-get install python3-pip -y
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED
RUN pip3 install flask
RUN pip3 install flask_cors

CMD ["python3", "api.py"]
