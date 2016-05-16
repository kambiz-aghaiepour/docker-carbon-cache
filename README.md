# docker-carbon-cache

centos7 based docker image for python-carbon

Suitable for collecting data via collectd, typical usage would be to start with external volume, e.g.:

```docker run -d \
--name carbon-cache \
-p 2003:2003 \
-v /data/carbon/whisper:/var/lib/carbon/whisper \
kambiz/carbon-cache:0.9.15
```
