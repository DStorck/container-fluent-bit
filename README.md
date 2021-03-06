# container-fluent-bit
"[Fluent Bit](http://fluentbit.io/) is an open source and multi-platform Log Forwarder which allows you to collect data/logs from different sources, unify and send them to multiple destinations."

The [container-fluent-bit](https://github.com/samsung-cnct/container-fluent-bit) repo contains a Dockerfile (and Jenkinsfile) to build (and test) the [`quay.io/samsung_cnct/fluent-bit`](https://quay.io/repository/samsung_cnct/fluent-bit) container. 

This container is used by the [chart-fluent-bit](https://github.com/samsung-cnct/chart-fluent-bit) repo, among others. See the chart repo for information on installing and configuring Fluent Bit on Kubernetes. The [fluent-bit.conf](https://github.com/samsung-cnct/container-fluent-bit/blob/master/fluent-bit.conf) included with the container artifact is intended for debugging only. 

Deployments to Kubernetes should use a [ConfigMap](https://kubernetes.io/docs/tasks/configure-pod-container/configmap/). For an example, from the chart repo, see [fluent-bit.yaml](https://github.com/samsung-cnct/chart-fluent-bit/tree/master/fluent-bit/templates).
