FROM rsyslog/rsyslog_dev_base_ubuntu:22.04

EXPOSE 514

VOLUME [ "/var/log", "/etc/rsyslog.d" ]

COPY rsyslog.conf /etc/rsyslog.conf

ENTRYPOINT [ "rsyslogd", "-n" ]