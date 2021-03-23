Logstash exporter
=================

Prometheus exporter for metrics provided by Node Stats API of Logstash.
> Pull requests to https://github.com/alxrem/prometheus-logstash-exporter

Building and running
--------------------

    go get gitlab.com/alxrem/prometheus-logstash-exporter
    cd ${GOPATH-$HOME/go}/src/gitlab.com/alxrem/prometheus-logstash-exporter
    go build
    ./prometheus-logstash-exporter <flags>

To see all available configuration flags:
```
./prometheus-logstash-exporter -h
```
- `web.listen-address` exporter listen port
- `web.telemetry-path` exporter telemetry path
- `logstash.address` logstash listen host, `localhost:9600`,char ',' split multi logstash host
- `logstash.timeout` logstash request timeout
- `logstash.id` logstash metric namespace,char ',' split multi namespace 