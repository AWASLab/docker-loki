FROM debian:bookworm-slim

RUN apt-get update && \
    apt-get -y install rsyslog && \
    rm -rf /var/lib/apt/lists/*

EXPOSE 514/udp

VOLUME [ "/var/log", "/etc/rsyslog.d" ]

COPY rsyslog.conf /etc/rsyslog.conf

ENTRYPOINT [ "rsyslogd", "-n" ]