FROM centos:centos7

LABEL desc="php-sandbox composer"

RUN yum install -y epel-release
RUN yum install -y http://rpms.famillecollet.com/enterprise/remi-release-7.rpm
RUN yum update -y
RUN yum install -y --enablerepo=remi-php80 php

RUN php -r "readfile('http://getcomposer.org/installer');" | php -- --version=2.0.11 --install-dir=/usr/bin/ --filename=composer && \
    yum install -y git zip