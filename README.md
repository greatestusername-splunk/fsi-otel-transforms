# fsi-otel-transforms

This repo contains a [values.yaml](./fsi-values.yaml) and an [ansible.yaml](./ansible.yaml) for modifying an Splunk4Rookies - Observability workshop into an FSI Vertical oriented workshop with APM/Metrics/Logs for a "Wire Transfer Service".

**NOTE:** This is not a new demo, it uses hipstershop as a deployment and then uses otel transforms in the collector to modify service names, endpoints, peer and url dimensions, etc before they hit ingest.

## To Use
1. Copy `fsi-values.yaml` to your splunk4rookies - observability workshop instance as `values.yaml`
2. Copy `ansible.yaml` to your splunk4rookies - observability workshop instance as `ansible.yaml`
3. run `ansible-playbook ansible.yaml`
4. Wait for metrics/traces/logs/etc to ingest