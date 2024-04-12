# Promptail -> Loki -> Grafana
- Promptail: ship log from file path to loki
- Loki: Log aggregation system
- Grafana: Monitoring tool

## Running docker compose
```sh
docker compose up -d
```

# Logstash + Promtail -> Loki -> Grafana
```sh
docker run -v ./logstash:/home/logstash/ --network loki --name logstash-loki --rm grafana/logstash
```
* Can use logstash in docker compose and run it

# Access UI
default url: http://localhost:3000
username: admin
password: admin

# Download example json log
https://github.com/elastic/examples/blob/master/Common%20Data%20Formats/nginx_json_logs/README.md