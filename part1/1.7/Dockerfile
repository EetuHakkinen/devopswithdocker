FROM ubuntu:16.04

WORKDIR /usr/bin/
RUN apt-get update
RUN apt-get install -y curl
COPY script.sh .
RUN ["chmod", "+x", "/usr/bin/script.sh"]

CMD ["/usr/bin/script.sh"]
