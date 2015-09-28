FROM rainetech/hadoop-core

COPY hdfs-site.xml /opt/hadoop-2.7.1/etc/hadoop/hdfs-site.xml

RUN \
  mkdir -p /data/hdfs && \
  useradd hdfs -g hadoop && \
  chown -R hdfs:hadoop /data/hdfs
