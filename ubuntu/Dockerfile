FROM ubuntu:18.04

MAINTAINER Anton Lebedev <mailbox@lebster.me>

# Install Cron
RUN apt-get update
RUN apt-get -y install cron

# Add crontab file in the cron directory
COPY crontab /etc/cron.d/crontab

# Give execution rights on the cron job
RUN chmod 0644 /etc/cron.d/crontab

# Apply cron job
RUN /usr/bin/crontab /etc/cron.d/crontab

CMD ["cron", "-f"]
