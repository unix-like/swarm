FROM centos:6.9

RUN yum install -y \
    epel-release.noarch \
 && yum install -y \
    libmcrypt-devel \
    freetype-devel \
    libpng-devel \
    libjpeg-turbo-devel \
    libmcrypt-devel \
 && yum clean all

COPY php /gotwo_data/Application/php

EXPOSE 9000

CMD ["/gotwo_data/Application/php/sbin/php-fpm"]
