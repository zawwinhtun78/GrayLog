# Overview

This is a mix of [graylog2 open-core](https://github.com/Graylog2/docker-compose/blob/main/open-core/docker-compose.yml) and [graylog2 docker install docs.](https://go2docs.graylog.org/5-0/downloading_and_installing_graylog/docker_installation.htm)

# Usage

````
git clone git@github.com:zawwinhtun78/GrayLog.git
````

```
docker compose up
```

Access graylog [here.](http://localhost:9000)

nxlog.conf is the Window NXLOG configuration for sending GELF format logs to Graylog. Replace the default C:\Program Files\nxlog\conf\nxlog.conf with the nxlog.conf and change the IP address to match your Graylog server.

**for the time issues**
edit in config/graylog/graylog.conf
root_timezone = SGT #you can change the timezone

edit docker-compose.yml
GRAYLOG_TIMEZONE: "Asia/Singapore"
TZ: "Asia/Singapore