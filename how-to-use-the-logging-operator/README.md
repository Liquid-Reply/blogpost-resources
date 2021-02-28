# Logging-Operator

This is our demo repository which is published with the [tutorial blogpost](https://liquidreply.net/howto-use-the-logging-operator).
It contains a customer_values.yaml which can be used to set up a log stream for all Kubernetes Namespaces that are not `kube-system, monitoring, logging, tracing` and a management_values.yaml that will collect logs from the named namespaces.

# Usage

Just install the `banzaicloud/logging-operator` helm-chart and the `banzaicloud/logging-operator-logging` helm-chart with these two values-files. 

# References
https://banzaicloud.com/docs/one-eye/logging-operator/

https://github.com/banzaicloud/logging-operator

https://liquidreply.net/howto-use-the-logging-operator
