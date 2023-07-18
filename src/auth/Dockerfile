# PLATFORM
FROM debian:buster
ENV PLATFORM PyFast3
RUN apt-get update && apt-get install -y python3 python3-dev python3-pip build-essential libffi-dev wait-for-it
# AUTH
COPY ./ /opt/auth
WORKDIR /opt/auth
RUN pip3 install -r requirements.txt


EXPOSE 5000

CMD [ "python3" ,"main.py" ]