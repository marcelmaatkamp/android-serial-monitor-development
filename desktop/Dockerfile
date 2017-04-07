FROM marcelmaatkamp/alpine-xfce4-xrdp
USER root
RUN apk update \
 && apk add git \
 && rm -rf /tmp/* /var/cache/apk/*
USER alpine
WORKDIR /home/alpine
ENV DOCKER_HOST=tcp://docker:2375
RUN git clone https://github.com/felHR85/UsbSerial.git
USER root
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
CMD ["/usr/sbin/docker-entrypoint.sh", "/usr/sbin/sshd", "-D"]
