# basic image
FROM ubuntu:18.04
# image creator
MAINTAINER bardroh
# key=value
LABEL "course"="KOSA"
# run command inside container
RUN apt-get update
RUN apt-get install apache2 -y
# add files
ADD test.html /var/www/html
# change working directory
WORKDIR /var/www/html
RUN ["/bin/bash", "-c", "echo hello >> test2.html"]
EXPOSE 80
CMD apachectl -DFOREGROUND

