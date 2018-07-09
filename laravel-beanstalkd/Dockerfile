FROM alpine

LABEL maintainer="Nguyen Thinh Hung <hungnt.dev@gmail.com>"

RUN apk add --no-cache beanstalkd

EXPOSE 11300
ENTRYPOINT ["/usr/bin/beanstalkd"]
