FROM alpine

LABEL maintainer="Nguyen Thinh Hung <hungnt.dev@gmail.com>"

# Install cron
RUN apk update && apk add dcron curl wget rsync ca-certificates && rm -rf /var/cache/apk/*

# Add crontab file in the cron directory
ADD .crontab /etc/cron.d/crontab

# Give execution rights on the cron job
RUN chmod 0644 /etc/cron.d/crontab

# Create the log file to be able to run tail
RUN touch /var/log/cron.log

# Run the command on container startup
CMD crond && tail -f /var/log/cron.log
