# Dutchie chart patches

This fork is a temporary delivery vehicle for chart changes that have not yet
been released upstream. Langfuse application images and source remain stock.

## `2.1.0-dutchie.1`

Adds `clickhouse.keeper.settings` pass-through to
`KeeperCluster.spec.settings`, matching the existing
`clickhouse.cluster.settings` pattern.

- Upstream proposal: https://github.com/langfuse/langfuse-k8s/pull/415
- Internal consumer: `GetDutchie/argocd-manifests`, stable Langfuse values
- Helm repository: https://getdutchie.github.io/langfuse-k8s
- Retirement condition: switch the consumer back to the first upstream chart
  release containing the setting, then archive or delete this fork.

No other downstream chart behavior should be added without explicit review.
