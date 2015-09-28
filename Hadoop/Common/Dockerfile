FROM rainetech/supervisor

RUN \
	apt-get update && \
	apt-get -y install default-jre

ADD http://www.eu.apache.org/dist/hadoop/common/hadoop-2.7.1/hadoop-2.7.1.tar.gz /opt/

RUN /
  cd /opt && \
  tar xvfz hadoop-2.7.1.tar.gz && \
	rm hadoop-2.7.1.tar.gz && \
	groupadd hadoop && \
	useradd hadoop -g hadoop && \
	chown -R hadoop:hadoop /opt/hadoop-2.7.1

COPY core-site.xml /opt/hadoop-2.7.1/etc/hadoop/core-site.xml
