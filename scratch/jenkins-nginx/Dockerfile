FROM nginx
MAINTAINER natalie

RUN apt-get -y update && apt-get -y upgrade
RUN apt-get -y install wget git

RUN rm /etc/nginx/conf.d/default.conf
RUN rm /etc/nginx/conf.d/example_ssl.conf

COPY conf/jenkins.conf /etc/nginx/conf.d/jenkins.conf
COPY conf/nginx.conf /etc/nginx/nginx.conf

EXPOSE 80

# RUN git clone https://github.com/letsencrypt/letsencrypt /opt/letsencrypt
# WORKDIR /root
# RUN tar xfv google-cloud-sdk-107.0.0-linux-x86.tar.gz

# ADD ./nginx.conf /etc/nginx.conf

