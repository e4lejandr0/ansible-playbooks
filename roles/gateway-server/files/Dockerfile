FROM centos:centos7

RUN yum upgrade -y

RUN yum install -y httpd

ENTRYPOINT /usr/sbin/httpd $OPTIONS -DFOREGROUND
