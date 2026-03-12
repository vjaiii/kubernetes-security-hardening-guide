# Kubernetes Hardening Checklist

## Access

- RBAC reviewed
- Admin access limited
- Service accounts scoped correctly

## Workloads

- Images come from trusted sources
- Containers do not run as root unless required
- Security context defined
- Resource limits configured

## Secrets

- Secrets access restricted
- Sensitive values not hardcoded in manifests
- Secret rotation process exists

## Network

- Network policies defined
- Unnecessary ingress paths blocked
- Internal services not broadly exposed

## Monitoring

- Audit logging enabled
- Runtime alerts configured
- Suspicious container behavior monitored
