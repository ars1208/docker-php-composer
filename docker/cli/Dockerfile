FROM --platform=linux/x86_64 centos:centos7

LABEL desc="php-sandbox cli"

RUN yum install -y epel-release
RUN yum install -y http://rpms.famillecollet.com/enterprise/remi-release-7.rpm
RUN yum update -y ca-certificates
RUN yum install -y --enablerepo=remi-php80 php