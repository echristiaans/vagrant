FROM centos:7
MAINTAINER Erik Christiaans <erik.christiaans@sentia.com>
RUN yum update -y
#RUN yum install wget -y
#ENTRYPOINT ["wget", "-O-", "-q"]
RUN yum groupinstall 'Development Tools' -y
COPY hello.c /root/
RUN gcc /root/hello.c -o /usr/local/bin/hello; chmod 755 /usr/local/bin/hello
CMD /usr/local/bin/hello
