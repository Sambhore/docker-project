FROM ubuntu:12.04
MAINTAINER sachin
RUN apt-get install -y apache* && apt-get clean && rm -rf /var/lib/apt/list/*

ENV APACHE_RUN_USER webuser
ENV APACHE_RUN_GROUP webuser
ENV APACHE_LOG_DIR /var/log/apache2/

EXPOSE 80

CMD ["/usr/sbin/apache2", "-D", "FOREGROUND"]
