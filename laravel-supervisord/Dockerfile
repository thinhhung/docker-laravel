FROM alpine

LABEL maintainer="Nguyen Thinh Hung <hungnt.dev@gmail.com>"

RUN apk add --no-cache supervisor

ENTRYPOINT ["/usr/bin/supervisord"]
