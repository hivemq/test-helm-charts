# HiveMQ Helm Repository

## Add the HiveMQ Helm repository

```bash
helm repo add test-hivemq https://hivemq.github.io/test-helm-charts/
```
## Install the HiveMQ Platform Operator
This will install a Hivemq Platform Operator for a Kubernetes cluster
```
helm upgrade --install hivemq-platform-operator test-hivemq/hivemq-platform-operator
```
## Install the HiveMQ Platform 
This will install a Hivemq Platform with 2 nodes for evaluation.
```
helm upgrade --install hivemq-platform test-hivemq/hivemq-platform

## Install the HiveMQ operator

This will install the HiveMQ operator as well as a custom resource that deploys a small 3-node evaluation cluster by default.

```
helm upgrade --install hivemq test-hivemq/hivemq-operator
```

For more information on configuring a cluster and advanced usage, visit the [HiveMQ Operator documentation](https://www.hivemq.com/docs/operator/).

## Install HiveMQ Swarm

This will install HiveMQ with one commander and three agents by default.

```
helm upgrade --install swarm test-hivemq/hivemq-swarm
```

For more information on configuring HiveMQ Swarm and advanced usage, visit [HiveMQ Swarm documentation](https://www.hivemq.com/docs/swarm/).
