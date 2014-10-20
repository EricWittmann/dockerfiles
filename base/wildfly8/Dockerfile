FROM centos:latest

MAINTAINER Eric Wittmann <eric.wittmann@redhat.com>

RUN yum -y install wget \
 && yum -y install java \
 && yum -y install unzip
RUN mkdir -p /home/overlord \
 && cd /home/overlord \
 && wget http://download.jboss.org/wildfly/8.1.0.Final/wildfly-8.1.0.Final.zip \
 && unzip wildfly-8.1.0.Final.zip

WORKDIR /home/overlord/wildfly-8.1.0.Final
CMD ["/home/overlord/wildfly-8.1.0.Final/bin/standalone.sh", "-b", "0.0.0.0", "-c", "standalone-full.xml"]

