
# Grafana Alloy

## Overview
Grafana Alloy is an observability collector used to collect, process and forward telemetry data.

## Purpose
- Discover Kubernetes pods.
- Collect container logs.
- Attach Kubernetes metadata to logs.
- Forward logs to Grafana Loki.

## Architecture
Kubernetes Pods → Grafana Alloy → Grafana Loki → Grafana

## Deployment
- Deployment method: Argo CD
- Package manager: Helm
- Namespace: monitoring
- Workload type: DaemonSet

## Configuration
- values.yaml: Helm deployment configuration.
- config.alloy: Log collection and forwarding pipeline.

## Validation
- Alloy pods are running.
- Kubernetes pod discovery works.
- Nginx logs are collected.
- Logs are available in Loki.

## Status
Documentation prepared. Deployment pending.
