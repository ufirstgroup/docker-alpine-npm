FROM mhart/alpine-node:6.8.0

MAINTAINER Jean-Luc Geering <jeanluc.geering@ufirstgroup.com>

# install su-exec

RUN apk update && apk upgrade && apk add \
  su-exec=0.2-r0

USER root

WORKDIR "/workdir"

ENV WORKDIR "/workdir"
ENV HOMEDIR "/homedir"

VOLUME ["/workdir", "/homedir"]

COPY entrypoint.sh /

ENTRYPOINT ["/entrypoint.sh"]
CMD ["npm"]
