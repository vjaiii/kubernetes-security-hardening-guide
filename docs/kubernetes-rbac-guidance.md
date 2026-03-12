# Kubernetes RBAC Guidance

## Goal

Reduce excessive permissions and improve control over cluster access.

## Key principles

- Prefer least privilege roles
- Separate admin access from workload access
- Avoid broad cluster-wide permissions unless required
- Review service account permissions regularly
- Limit access to secrets and sensitive namespaces

## Common risks

- Overly broad ClusterRoleBindings
- Shared administrative accounts
- Excessive default namespace usage
- Unreviewed service account permissions

## Good practices

- Use namespace-scoped roles where possible
- Separate human access from workload identity
- Review privileged operations
- Log and review administrative activity
