
# Loki

## Overview
Grafana Loki is a log aggregation system used to store and query logs from Kubernetes workloads.

## Purpose
- Collect and store application logs.
- Query logs using LogQL.
- Integrate with Grafana for log visualization.
- Support troubleshooting and incident investigation.

## Architecture
Kubernetes Pods → Grafana Alloy → Loki → Grafana

## Deployment
- Deployment method: Argo CD
- Package manager: Helm
- Helm chart: grafana/loki
- Chart version: 7.7.0
- Deployment mode: SingleBinary
- Namespace: monitoring

## Configuration
The `values.yaml` file contains Loki Helm configuration, including storage, persistence, replication and deployment settings.

## Validation
After deployment, verify:
- Loki pod is running.
- Loki service is available.
- Loki is accepting log ingestion requests.
- Logs can be queried through Grafana.

## Status
Configuration prepared. Deployment pending.
