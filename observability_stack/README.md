# Observability Stack (Podman Compose)
For people who want to standup a full Observability stack in their homelab or for testing.

Stack Includes:
- Loki (logs)
- Prometheus (metrics)
- Alertmanager (alerts)
- Grafana (visualisation)

## Run
This is setup for SELinux based systems so might need tweaking, but I have tested on Rocky Linux, Debian and Windows all work without issues

### Interactive
podman compose up 
### Daemon 
podman compose up -d
### Shut it all down
podman compose down

## URLs are listening global so localhost or the hosting servers hostname
- Grafana: http://localhost:3000 (admin/admin)
- Prometheus: http://localhost:9090
- Alertmanager: http://localhost:9093
- Loki: http://localhost:3100
