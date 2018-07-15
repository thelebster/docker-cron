An example of running cron job in a docker container.

Check the https://crontab.guru to find more crontab expressions.

### Ubuntu 18.04

~125 Mb

```
docker build --rm -t thelebster/ubuntu-cron-example ./ubuntu
docker run -ti --rm --name ubuntu-cron-example -d thelebster/ubuntu-cron-example
```

### Alpine 3.8

~5 Mb

```
docker build --rm -t thelebster/alpine-cron-example ./alpine
docker run -ti --rm --name alpine-cron-example -d thelebster/alpine-cron-example
```
