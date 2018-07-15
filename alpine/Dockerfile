FROM alpine:3.8

MAINTAINER Anton Lebedev <mailbox@lebster.me>

# Add crontab file in the cron directory
COPY crontab /crontab

# Apply cron job
RUN crontab /crontab

CMD ["crond", "-f", "-L -"]
