FROM ubuntu

RUN \
	apt-get update && \
	apt-get -y install supervisor

VOLUME ["/var/log/supervisor"]

RUN \
	mkdir /var/lib/supervisor

COPY supervisord.conf /etc/supervisor/supervisord.conf
ENTRYPOINT ["supervisord", "-c", "/etc/supervisor/supervisord.conf"]