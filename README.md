# Production-Grade SRE Platform

## Overview
This project is a hands-on SRE / Platform Engineering lab focused on
building, operating, breaking, and hardening a production-grade,
event-driven backend system on Kubernetes.

The goal is not just to deploy services, but to own reliability,
observability, and safe operation under failure.

## What I’m Building
A small but realistic distributed system consisting of:
- An API service handling user requests
- Background workers processing events
- Event-driven communication (NATS)
- Kubernetes-based deployment
- CI/CD with safe deploy strategies
- Full observability (metrics, logs, traces)
- Defined SLIs, SLOs, and error budgets

## Why This Project Exists
Remote hiring has shifted toward engineers who can:
- Own production systems
- Prevent and handle incidents
- Design for failure
- Balance velocity with reliability

This project is designed to simulate real-world SRE responsibilities,
including incident response and postmortems.

## Non-Goals
- This is not a toy demo
- This is not a “learn Kubernetes basics” tutorial
- This is not multi-cloud for the sake of it

## Tech Stack (Initial)
- Runtime: Node.js or Bun
- Containers: Docker
- Orchestration: Kubernetes
- Events: NATS
- IaC: Terraform (infra), Ansible (config where needed)
- Observability: OpenTelemetry, Prometheus, Grafana, Loki
- CI/CD: GitHub Actions or GitLab CI

## Success Criteria
- Services survive restarts and failures
- Deployments do not cause user-visible downtime
- Incidents are detectable within minutes
- Postmortems result in concrete system improvements
