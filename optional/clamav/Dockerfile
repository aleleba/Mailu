FROM alpine:3.8

RUN apk add --no-cache clamav rsyslog wget clamav-libunrar

COPY conf /etc/clamav
COPY start.sh /start.sh

EXPOSE 3310/tcp
VOLUME ["/data"]

CMD ["/start.sh"]
