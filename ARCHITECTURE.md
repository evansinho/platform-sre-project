# High-Level Architecture

## Components
- API Service
  - Handles synchronous HTTP requests
  - Publishes events to NATS
- Worker Service
  - Consumes events from NATS
  - Performs background processing
- NATS
  - Event backbone
- Kubernetes
  - Schedules and runs services
- Observability Stack
  - Metrics, logs, traces
- CI/CD Pipeline
  - Builds, tests, and safely deploys services

## Failure Assumptions
- Pods will crash
- Nodes will be restarted
- Deployments will introduce bugs
- Dependencies will be slow or unavailable

The system is designed with the assumption that failure is normal.
