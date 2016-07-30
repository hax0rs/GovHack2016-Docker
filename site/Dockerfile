FROM debian:jessie
MAINTAINER Nick <nicko21.nvs@gmail.com>
RUN apt-get update
RUN apt-get install -y python3 python3-pip libffi-dev
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app
COPY ./app/requirements.txt requirements.txt
RUN pip3 install -r requirements.txt
EXPOSE 8080
CMD ["python3", "runserver.py"]
