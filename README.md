## Create Log monitoring with Grafana + Loki + Promtail

# Install Commands

```bash

git clone https://github.com/mayur-chavhan/Loki-Promtail-Grafana.git
```
```
cd Loki-Promtail-Grafana
```
```
docker-compose up -d
```

# Add Promtail agents on remote server.

Install promtail binary or docker-compose file and update promtail config file for remote Loki server IP and restart promtail service.

promtail-config.yaml 

```
clients:
  - url: http://repalce_remote_server_ip_here:3100/loki/api/v1/push
```
