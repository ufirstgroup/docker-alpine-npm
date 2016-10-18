FROM mhart/alpine-node:6.8.1

MAINTAINER Jean-Luc Geering <jeanluc.geering@ufirstgroup.com>

# install bash, su-exec and tini

RUN apk update && apk upgrade && apk add \
  bash=4.3.42-r3 \
  su-exec=0.2-r0 \
  tini=0.9.0-r1

USER root

WORKDIR "/workdir"

ENV WORKDIR "/workdir"
ENV HOMEDIR "/homedir"

VOLUME ["/workdir", "/homedir"]

COPY entrypoint.sh /

ENTRYPOINT ["/sbin/tini", "--", "/entrypoint.sh"]
CMD ["npm"]
