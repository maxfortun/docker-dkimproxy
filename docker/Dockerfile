FROM alpine:edge

RUN echo https://dl-cdn.alpinelinux.org/alpine/edge/testing >> /etc/apk/repositories

RUN apk --update add dkimproxy

EXPOSE 10027/tcp

CMD [ "dkimproxy.out", "--conf_file=/etc/dkimproxy/dkimproxy_out.conf", "--daemonize" ]

