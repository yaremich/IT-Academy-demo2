FROM ubuntu:latest

ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get update
RUN apt-get -y upgrade
RUN apt install apache2 vim -y
RUN apt-get install -y libxml2-dev

RUN apt install php7.4 -y
RUN apt install php7.4-common php7.4-mysql php7.4-xml php7.4-xmlrpc php7.4-curl \
    php7.4-gd php7.4-imagick php7.4-cli php7.4-dev php7.4-imap php7.4-mbstring \
    php7.4-opcache php7.4-soap php7.4-zip php7.4-intl -y

#RUN chmod -R 777 system/storage/cache/ \
#    system/storage/download/ \
#    system/storage/logs/ \
#    system/storage/modification/ \
#    system/storage/session/ \
#    system/storage/upload/ \
#    system/storage/vendor/ \
#    image/ \
#    image/cache/ \
#    image/catalog/ \
#    config.php \
#    admin/config.php 




# By default, simply start apache.
CMD /usr/sbin/apache2ctl -D FOREGROUND

