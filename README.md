An example of running cron job in a docker container.

Check the https://crontab.guru to find more crontab expressions.

```
docker build --rm -t thelebster/cron-example ./ubuntu
docker run -ti thelebster/cron-example
```
