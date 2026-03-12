# Network Policy Patterns

## Purpose

Kubernetes network policies help limit which workloads can communicate with each other.

## Recommended approach

- Deny unnecessary east-west traffic
- Explicitly allow only required application paths
- Protect backend services from unrestricted namespace access
- Restrict access to platform and management components

## Typical policy goals

Frontend can talk to API

API can talk to database

Monitoring namespace can scrape workloads

Other namespaces cannot connect by default

## Review questions

- Which pods truly need inbound access
- Are sensitive services isolated
- Are management endpoints protected
- Is cross-namespace traffic intentional
